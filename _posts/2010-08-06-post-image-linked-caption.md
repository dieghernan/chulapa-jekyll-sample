---
title: "Post: Image (Linked with Caption)"
categories:
  - Post Formats
tags:
  - image
  - Post Formats
---

{% capture fig_img %}
[![Foo](https://picsum.photos/seed/10/600/300)](https://picsum.photos/seed/10/600/300)
{% endcapture %}

{% capture fig_caption %}
Stairs? Were we're going we don't need no stairs.
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>{{ fig_caption | markdownify | remove: "<p>" | remove: "</p>" }}</figcaption>
</figure>