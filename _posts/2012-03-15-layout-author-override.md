---
title: "Layout: Author Override"
author: 
  name: Billy Rick
  avatar      : "images/foo-bar-identity-th.jpg"
  links:
    - url: http://thewhip.com
      icon: "fa fa-blog"
      label: GitHub
    - url: billy@rick.com
      icon: "fa fa-envelope"
      label: Email
excerpt: "A post to test author overrides using a data file."
---

Sites that may have content authored from various individuals .

To attribute an author to a post or page that is different from the site author specified in `_config.yml`,
use this post yaml:

```yaml
author: 
  name: Billy Rick
  avatar      : "images/foo-bar-identity-th.jpg"
  links:
    - url: http://thewhip.com
      icon: "fa fa-blog"
      label: GitHub
    - url: billy@rick.com
      icon: "fa fa-envelope"
      label: Email
```
