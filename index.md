---
layout: default
---

# Projects

---

{% tabs projects %}

<!-- All projects -->
{% tab projects All%}

{% for project in site.projects %}
    {{ project.content | markdownify }}
    ---
{% endfor %}

{% endtab %}

<!-- Data Engineer projects -->
{% tab projects Data Engineer %}

{% for project in site.projects %}
    {% if project.tab == "data-engineer" %}

        {{ project.content | markdownify }}
        ---

    {% endif %}
{% endfor %}

{% endtab %}

<!-- Python projects -->
{% tab projects Python %}

{% for project in site.projects %}
    {% if project.tab == "python" %}
        {{ project.content | markdownify }}
        ---
    {% endif %}
{% endfor %}

{% endtab %}

{% endtabs %}

---
