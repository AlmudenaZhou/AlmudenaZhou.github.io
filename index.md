---
layout: default
---

<h1>Projects</h1>

<hr>


{% if page.selectedTags %}
  {% assign selectedTags = page.selectedTags | split: "," %}
{% else %}
  {% assign selectedTags = "" %}
{% endif %}

{% tabs projects %}

<!-- All projects -->
{% tab projects All%}
<ul>
  {% for project in site.projects %}
    {% if page.selectedTags != "" %}
      {% if project.tags contains page.selectedTags %}
        <li>
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        </li>
        <hr>
      {% endif %}
    {% else %}
        <li>
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        </li>
        <hr>
    {% endif %}
  {% endfor %}
</ul>

{% endtab %}

<!-- Data Engineer projects -->
{% tab projects Data Engineer %}

<ul>
  {% for project in site.projects %}
    {% if project.category == "data-engineer" %}
      {% if page.selectedTags != "" %}
        {% if project.tags contains page.selectedTags %}
          <li>
          <h2>{{ project.title }}</h2>
          <p>{{ project.content | markdownify }}</p>
          </li>
          <hr>
        {% endif %}
      {% else %}
          <li>
          <h2>{{ project.title }}</h2>
          <p>{{ project.content | markdownify }}</p>
          </li>
          <hr>
      {% endif %}
    {% endif %}
  {% endfor %}
</ul>

{% endtab %}

<!-- Python projects -->
{% tab projects Python %}

<ul>
  {% for project in site.projects %}
    {% if project.category == "python" %}
      {% if page.selectedTags != "" %}
        {% if project.tags contains page.selectedTags %}
          <li>
          <h2>{{ project.title }}</h2>
          <p>{{ project.content | markdownify }}</p>
          </li>
          <hr>
        {% endif %}
      {% else %}
          <li>
          <h2>{{ project.title }}</h2>
          <p>{{ project.content | markdownify }}</p>
          </li>
          <hr>
      {% endif %}
    {% endif %}
  {% endfor %}
</ul>

{% endtab %}

{% endtabs %}

---
