---
layout: default
title: Bootstrap Demo
subtitle: BS4 components
excerpt: Demo on Boostrap 4
date: 2015-03-04
last_modified_at: 2018-02-08
tags: [skin, bootstrap, themes-guide, layout, image, html, css]
categories: [skins]
show_bottomnavs: true
show_tags: true
show_categories: true
show_toc: true
permalink: /bootstrap4
show_breadcrumb: true
show_date         : true
show_sociallinks  : true
show_comments     : true
show_related      : true
show_random       : true
show_author       : true
show_sidetoc      : true
show_seo          : true
breadcrumb_list:
  - label: Home
    url: /
  - label: Sitemap
    url: /sitemap/#pages
---



{% if page.show_bottomnavs -%}
{% include components/navbeforeafter.html -%}
{% endif -%}
{% if page.show_categories -%}
{% include components/categories.html-%}
{% endif -%}
{% if page.show_tags -%}
{% include components/tags.html-%}
{% endif -%}


{% include snippets/bootstrapdemo.html  %}