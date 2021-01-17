---
layout: default
---

# Articles

<p>
{% for post in site.categories.articles %}  
<h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>  
<time>{{ post.date | date: "%b %-d, %Y" }}</time>  
{% endfor %}
</p>

## html just html
