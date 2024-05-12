---
layout: default
---

<h1>Projects</h1>

<hr>


{% assign selectedTags = page.selectedTags | split: "," %}

{% tabs projects %}

<!-- All projects -->
{% tab projects All%}
{% assign selectedTags = page.selectedTags | split: "," %}
<ul>
  {% for project in site.projects %}
    {% for tag in selectedTags %}
        {% if tag in project.tags %}
        <li>
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        </li>
        <hr>
        {% endif %}
    {% endfor %}
  {% endfor %}
</ul>

{% endtab %}

<!-- Data Engineer projects -->
{% tab projects Data Engineer %}

<ul>
  {% for project in site.projects %}
    {% if project.category == "data-engineer" %}
    {% for tag in selectedTags %}
        {% if tag in project.tags %}
        <li>
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        </li>
        <hr>
        {% endif %}
    {% endfor %}
    {% endif %}
  {% endfor %}
</ul>

{% endtab %}

<!-- Python projects -->
{% tab projects Python %}

<ul>
  {% for project in site.projects %}
    {% if project.category == "python" %}
    {% for tag in selectedTags %}
        {% if tag in project.tags %}
        <li>
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        </li>
        <hr>
        {% endif %}
    {% endfor %}
    {% endif %}
  {% endfor %}
</ul>

{% endtab %}

{% endtabs %}

---
