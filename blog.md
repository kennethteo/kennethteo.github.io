---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---
<h2>Blog</h2>
<ul>
    {% assign filtered_posts = site.posts | where: 'categories', 'blog' %}
    {% for post in filtered_posts %}
    <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>