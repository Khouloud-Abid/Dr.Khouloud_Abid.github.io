---
layout: archive
title: "My Publications"
permalink: /publications/
author_profile: true
---

---
title: "Publications"
permalink: /publications/
author_profile: true
---

## Publications

{% assign pubs = site.publications | sort: 'date' | reverse %}

{% for post in pubs %}

### {{ post.title }}

**{{ post.date | date: "%Y" }}** · *{{ post.venue }}*

{% if post.paperurl %}
[📄 Paper]({{ post.paperurl }})
{% endif %}

{% if post.doi %}
[DOI](https://doi.org/{{ post.doi }})
{% endif %}

{% endfor %}
---





