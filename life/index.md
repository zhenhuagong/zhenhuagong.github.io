---
layout: home
---

<div class="index-content life">
    <div class="section">
        <ul class="artical-cate">

            <li><a href="/blog.html"><span>Tech</span></a></li>
            <li class="on" style="text-align:center"><a href="/life"><span>Life</span></a></li>
            <li style="text-align:right"><a href="/me"><span>About Me</span></a></li>


        </ul>

        <div class="cate-bar"><span id="cateBar"></span></div>

        <ul class="artical-list">
        {% for post in site.categories.life %}
            <li>
                <h2>
                    <a href="{{ post.url }}">{{ post.title }}</a>
                </h2>
                {{ post.date | date_to_string}}
                <div class="title-desc">{{ post.description }}</div>
            </li>
        {% endfor %}
        </ul>
    </div>
    <div class="aside">
    </div>
</div>
