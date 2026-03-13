---
layout: default
title: Thomas Yu
---

# Thomas Yu

Working on data systems, infrastructure, and AI workflows.

[LinkedIn](https://www.linkedin.com/in/thomasyu888/) · [GitHub](https://github.com/thomasyu888)

---

## Blog

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
<span>{{ post.date | date: "%B %-d, %Y" }}</span>

{{ post.excerpt }}

{% endfor %}
