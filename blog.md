---
layout: default
permalink: /blog/
level: "../"
---

# Tất cả bài đăng
---

{% assign count = '0' %}
{% for post in site.posts %}
&bull; ({{ site.posts | size | minus: count }}) &rarr; [{{ post.title }}](..{{ post.url }})
{% capture count %}{{ count | plus: '1' }}{% endcapture %}
{% endfor %}

---
