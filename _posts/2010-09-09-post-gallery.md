---
title: "Post: Gallery"
categories:
  - Post Formats
tags:
  - gallery
  - Post Formats
  - tiled
---

These are gallery tests for image wrapped in `<figure>` elements.

And then drop-in the gallery include --- gallery `caption` is optional.

```liquid
{% raw %}
{% assign externalgallery = "
https://picsum.photos/seed/10/600/1200,
https://picsum.photos/seed/20/800/500,
https://picsum.photos/seed/30/900/1200,
https://picsum.photos/seed/40/900/1300,
https://picsum.photos/seed/50/750/325,
https://picsum.photos/seed/60/600,
https://picsum.photos/seed/70/700/500" %}

{% include_cached snippets/masonry.html external=externalgallery %}{% endraw %}
```

{% assign externalgallery = "
https://picsum.photos/seed/10/600/1200,
https://picsum.photos/seed/20/800/500,
https://picsum.photos/seed/30/900/1200,
https://picsum.photos/seed/40/900/1300,
https://picsum.photos/seed/50/750/325,
https://picsum.photos/seed/60/600,
https://picsum.photos/seed/70/700/500" %}

{% include_cached snippets/masonry.html external=externalgallery %}

This is some text after the gallery just to make sure that everything aligns properly.

Here comes another gallery.
```liquid
{% raw %}
{% include_cached snippets/masonry.html internal="images" %}
{% endraw %}
```

{% include_cached snippets/masonry.html internal="images" %}

And for giggles a carousel

```liquid
{% raw %}
{% include_cached snippets/carousel.html internal="images" controls="true" indicators="true" %}
{% endraw %}

```

{% include_cached snippets/carousel.html internal="images" controls="true" indicators="true" %}
