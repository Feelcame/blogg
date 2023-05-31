---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---


---

- "site.baseurl": `{{ site.baseurl }}`
- "pages_hostname": `{{ site.github.pages_hostname }}`
- "owner_name": `{{ site.github.owner_name }}`
- "repository_name": `{{ site.github.repository_name }}`
- "url" (or the CNAME): `{{ site.github.url }}`

---

- "baseur (my):" 
{% unless site.github.repository_name == (site.github.owner_name | downcase | append: ".github.io") or (site.github.url | split: "/" | size < 3  ) %}
{{ site.github.repository_name | prepend: "/" }}
{% endunless %}

- `site.github.owner_name | downcase | append: ".github.io"`: {{ site.github.owner_name | downcase | append: ".github.io" }}
- `site.github.url | split: "/" | size`: {{ site.github.url | split: "/" | size }} 
