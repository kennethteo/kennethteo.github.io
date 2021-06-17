---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---
<h2>Tech</h2>
<ul>
    {% for post in site.posts %}
    {% if post.categories contains "tech" %}
    <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endif %}
    {% endfor %}
</ul>