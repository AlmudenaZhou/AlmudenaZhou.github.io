---
layout: default
---

# Projects

---

{% tabs projects %}

<!-- All projects -->
{% tab projects All%}

{% for project in site.projects %}
    <h2>{{ project.title }}</h2>
    <p>{{ project.content | markdownify }}</p>
    <hr>
{% endfor %}

{% endtab %}

<!-- Data Engineer projects -->
{% tab projects Data Engineer %}

{% for project in site.projects %}
    {% if project.tab = "data-engineer" %}
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        <hr>
{% endfor %}

{% endtab %}

<!-- Python projects -->
{% tab projects Python %}

{% for project in site.projects %}
    {% if project.tab = "python" %}
        <h2>{{ project.title }}</h2>
        <p>{{ project.content | markdownify }}</p>
        <hr>
{% endfor %}

{% endtab %}

{% endtabs %}

---
