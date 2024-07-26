---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Hello world

Bonjour à tous.
Voici quelques tests avec Jekyll

# Nouveau billet

Voici un autre tests.

{% for staff_member in site.staff_members %}
  <h2>
    <a href="{{ staff_member.url }}">
      {{ staff_member.name }} - {{ staff_member.position }}
    </a>
  </h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
