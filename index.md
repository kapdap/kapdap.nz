{% for repository in site.github.public_repositories %}
* [{{ repository.name }}]({{ repository.html_url }})
  {% for release in repository.releases %}
  * [{{ release.name }}]({{ release.html_url }})
  {% endfor %}
{% endfor %}
