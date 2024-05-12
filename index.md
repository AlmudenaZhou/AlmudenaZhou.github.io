---
layout: default
---

<h1>Projects</h1>

<hr>

{% tabs projects %}

<!-- All projects -->
{% tab projects All%}

{% for project in site.projects %}
<ul>
  {% for author in site.authors %}
    <li>
      <h2>{{ project.title }}</h2>
      <p>{{ project.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>

{% endtab %}

<!-- Data Engineer projects -->
<!-- {% tab projects Data Engineer %}

{% for project in site.projects %}
    {% if project.tab == "data-engineer" %}

        {{ project.content }}
        ---

    {% endif %}
{% endfor %}

{% endtab %} -->

<!-- Python projects -->
<!-- {% tab projects Python %}

{% for project in site.projects %}
    {% if project.tab == "python" %}
        {{ project.content }}
        ---
    {% endif %}
{% endfor %}

{% endtab %} -->

{% endtabs %}

---
