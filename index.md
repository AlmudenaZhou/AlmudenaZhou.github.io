---
layout: default
---

<h1>Projects</h1>

<hr>

{% tabs projects %}

<!-- All projects -->
{% tab projects All%}

<ul>
  {% for project in site.projects %}
    <li>
      <h2>{{ project.title }}</h2>
      <p>{{ project.content | markdownify }}</p>
    </li>
    <hr>
  {% endfor %}
</ul>

{% endtab %}

<!-- Data Engineer projects -->
{% tab projects Data Engineer %}

<ul>
  {% for project in site.projects %}
    {% if project.category == "data-engineer" %}
        <li>
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

<ul>
  {% for project in site.projects %}
    {% if project.category == "python" %}
        <li>
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        </li>
        <hr>
    {% endif %}
  {% endfor %}
</ul>

{% endtab %}

{% endtabs %}

---
