---
layout: default
---

<h1>Projects</h1>

<hr>

{% tabs projects %}

<!-- All projects -->
{% tab projects All %}
<ul id="allProjects">
  {% for project in site.projects %}
    <li data-tags="{{ project.tags | join: ',' }}">
      <h2>{{ project.title }}</h2>
      <p>{{ project.content | markdownify }}</p>
    </li>
    <hr>
  {% endfor %}
</ul>
{% endtab %}

<!-- Data Engineer projects -->
{% tab projects Data Engineer %}
<ul id="dataEngineerProjects">
  {% for project in site.projects %}
    {% if project.category == "data-engineer" %}
      <li data-tags="{{ project.tags | join: ',' }}">
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
      </li>
      <hr>
    {% endif %}
  {% endfor %}
</ul>
{% endtab %}

<!-- Python projects -->
{% tab projects Python %}
<ul id="pythonProjects">
  {% for project in site.projects %}
    {% if project.category == "python" %}
      <li data-tags="{{ project.tags | join: ',' }}">
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
      </li>
      <hr>
    {% endif %}
  {% endfor %}
</ul>
{% endtab %}

{% endtabs %}

<script>
document.addEventListener("DOMContentLoaded", function () {
  var projects = document.querySelectorAll('[data-tags]');
  var searchInput = document.getElementById('search-bar-multi-select');

  searchInput.addEventListener('input', function() {
    var filter = searchInput.value.trim().toLowerCase();
    projects.forEach(function(project) {
      var tags = project.getAttribute('data-tags').split(',');
      var showProject = tags.some(function(tag) {
        return tag.trim().toLowerCase().includes(filter);
      });
      project.style.display = showProject ? '' : 'none';

    });
  });
});
</script>