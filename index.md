---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---
# Project Pages
{% include search-lunr.html %}
{% for repository in site.github.public_repositories %}
{% if repository.has_pages == true %}
# [{{ repository.name }}]({{ repository.html_url }}) 
{{ repository.description }}
###### Topics : {% for topic in repository.topics %}{{ topic }}{% if forloop.last %}{% else %}, {% endif %}{% endfor %}
{% endif %}
{% endfor %}
