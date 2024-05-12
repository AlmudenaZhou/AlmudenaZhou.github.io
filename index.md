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

<p>{{selectedTags}}</p>

{% tabs projects %}

<!-- All projects -->
{% tab projects All%}
<ul>
  {% for project in site.projects %}
    {% if selectedTags != "" %}
      {% if project.tags contains selectedTags %}
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
      {% if selectedTags != "" %}
        {% if project.tags contains selectedTags %}
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
      {% if selectedTags != "" %}
        {% if project.tags contains selectedTags %}
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
