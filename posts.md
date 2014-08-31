---
layout: about
title: Blog Posts
navbar: blog
---

Blog Posts
==========

| Title | Author | Date |
| ----- | ------ | ---- | {% for post in site.posts %}
| [{{ post.title }}]({{ post.url }}) |{{ post.author }} | {{ post.date | date: "%A %B %-d, %Y" }} |{% endfor %}
{: .table .table-hover .table-striped}
