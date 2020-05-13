---
title: Training
layout: page
---

{% for repository in site.github.public_repositories %}
{% if repository.topics contains "training" %}
# [{{ repository.name }}]({{ repository.html_url }}) 
{{ repository.description }}
###### Topics : {% for topic in repository.topics %}{{ topic }}{% if forloop.last %}{% else %}, {% endif %}{% endfor %}
{% endif %}
{% endfor %}