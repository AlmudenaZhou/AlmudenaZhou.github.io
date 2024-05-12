---
layout: default
---

<h1>Projects</h1>

<hr>

<!-- Priority order of the projects from _config.yml -->
{% assign ordered_projects = '' | split: '' %}
{% if site.projects-order %}
    {% for project in site.projects-order %}
        {% assign project-elem = site.projects | where: "short_title", project %}
        {% assign ordered_projects = ordered_projects | concat: project-elem %}
    {% endfor %}
{% else %}
    {% assign ordered_projects = site.projects %}
{% endif %}

<p>{{ ordered_projects }}<p>

{% tabs projects %}

<!-- All projects -->
{% tab projects All %}
<ul id="allProjects">
  {% for project in ordered_projects %}
    <li class="ind-project" data-tags="{{ project.tags | join: ',' }}">
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
  {% for project in ordered_projects %}
    {% if project.category == "data-engineer" %}
      <li  class="ind-project" data-tags="{{ project.tags | join: ',' }}">
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
  {% for project in ordered_projects %}
    {% if project.category == "python" %}
      <li  class="ind-project" data-tags="{{ project.tags | join: ',' }}">
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
      </li>
      <hr>
    {% endif %}
  {% endfor %}
</ul>
{% endtab %}

{% endtabs %}

<!-- Filter the projects by tag -->
<script>
document.addEventListener("DOMContentLoaded", function () {
  var projects = document.querySelectorAll('.ind-project');
  var select = document.getElementById("tagSelect");

    console.log("projects: ", projects)
    select.addEventListener('change', function() {
    var filter = select.value.trim().toLowerCase();
    projects.forEach(function(project) {
      var tags = project.getAttribute('data-tags').split(',');
      var showProject = tags.some(function(tag) {
        return tag.trim().toLowerCase().includes(filter);
      });
        console.log("Filter:", filter);
        console.log("Tags:", tags);
        console.log("Show project:", showProject);
      project.style.display = showProject ? '' : 'none';
    });
    console.log("change")
  });
});
</script>