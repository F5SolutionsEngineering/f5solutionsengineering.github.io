---
title: Public Repositories
layout: page
---

{% for repository in site.github.public_repositories %}
  # [{{ repository.name }}]({{ repository.html_url }}) 
  #### Destription: {{ repository.description }}
  ###### Topics : {% for topic in repository.topics %}{{ topic }}{% if forloop.last %}{% else %}, {% endif %}{% endfor %}
{% endfor %}