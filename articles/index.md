---
layout: default
---

# Articles

<p>
{% for post in site.categories.articles %}  
<time>{{ post.date | date: "%b %-d, %Y" }}</time>  
<h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>  
{% endfor %}
</p>

## html just html
