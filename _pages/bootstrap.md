---
layout: default
title: Bootstrap Demo
subtitle: BS4 components
excerpt: Demo on Boostrap 4
date: 2015-03-04
last_modified_at: 2018-02-08
tags: [skin, bootstrap, themes-guide]
categories: [skins]
show_bottomnavs: true
show_tags: true
show_categories: true
permalink: /bootstrap4
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