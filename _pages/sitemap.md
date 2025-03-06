---
title: "Sitemap"
permalink: /sitemap/
author_profile: false
show_toc: true
---

{% include base_path %}


A list of all the posts and pages found on the site. For you robots out there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.

<h2 id="pages">Pages</h2>
{% assign: mydocs = site.html_pages %}
{% include_cached components/simplelist.html cacheddocs=mydocs %}


<h2 id="posts">Posts</h2>

{% include_cached components/simplelist.html cacheddocs=site.posts %}

{% capture written_label %}'None'{% endcapture %}

<h2 id="collections">Collections</h2>
{% for collection in site.collections %}
{% unless collection.output == false or collection.label == "posts" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
  <h3 id="{{label}}">{{ label }}</h3>
  {% capture written_label %}{{ label }}{% endcapture %}
      {%- assign thiscol = site.documents | where_exp: "item", "item.collection == label" -%}
    {% include_cached components/simplelist.html cacheddocs=thiscol %}
    {% endif %}
{% endunless %}
{% endfor %}
