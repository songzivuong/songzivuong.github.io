---
layout: post
title: "Build a Tag Cloud in Jekyll"
date: 2019-02-20 16:52:28 +0800
categories: Programming
tags: jekyll tag
---

The tag archive is an important feature for a blog site. I have build a gem-based Jekyll theme [Minimax](https://github.com/songzivuong/jekyll-theme-minimax), which extends the default Jekyll theme [Minima](https://github.com/jekyll/minima). My first big step is implementing the tag cloud.

1. Create a template in `_includes/tag_cloud.html` for showing tag cloud.

    ```html
    {% raw %}
    <div class="tag-cloud">
    {% assign tags = site.tags | sort %}
    {% for tag in tags %}
        <span class="site-tag">
        <a href="/tag/{{ tag | first | slugify }}/"
            style="font-size: {{ tag | last | size  |  times: 4 | plus: 80  }}%">
                {{ tag[0] | replace:'-', ' ' }} 
        </a><sup>{{ tag | last | size }}</sup>
        </span>&nbsp;
    {% endfor %}
    </div>
    {% endraw %}
    ```

    The more number of tags, the bigger font size.

    In anywhere you want to show the tag cloud, just insert `{% raw %}{% include tag_cloud.html %}{% endraw %}`.

2. For each tag, make a page to list all posts that are labeled with the tag. You can manually make these pages, or you can write [a script](https://github.com/songzivuong/jekyll-theme-minimax/blob/master/scripts/tag-generator.py) to generate all tag pages.

    The layout of tag pages may be look like this:

    ```html
    {% raw %}
    ---
    layout: default
    ---
    <div class="post">
    <h1>Tag: {{ page.tag }}</h1>
    <ul>
    {% for post in site.tags[page.tag] %}
    <li>
        {{ post.date | date: "%Y-%m-%d" }} &raquo; <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
    </ul>
    </div>
    <hr>
    {% endraw %}
    ```
