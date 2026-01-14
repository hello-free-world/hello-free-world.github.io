---
category: research
title_en: Research
title_zh: 论文
layout: page
permalink: "/research/"
---

<div class="lang-content" id="en">
  <h2 class="post-list-heading">
	<a href="/">All</a>
	| <a href="/fiction/">Fiction</a>
	| <a href="/politics/">Politics</a>
	| Research
  </h2>
  <ul class="post-list">
    {% for post in site.categories.research %}
      <li>
	    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h3>
          <a class="post-link" href="{{ post.url }}">
		    {%- if post.title_en -%}
			  {{ post.title_en | escape }}
		    {%- else -%}
			  {{ post.title | escape }}
		    {%- endif -%}
          </a>
        </h3>
      </li>
    {% endfor %}
  </ul>
</div>

<div class="lang-content" id="zh">
  <h2 class="post-list-heading">
	<a href="/#lang=zh">全部</a>
	| <a href="/fiction/#lang=zh">漫剧</a>
	| <a href="/politics/#lang=zh">政论</a>
	| 论文
  </h2>
  <ul class="post-list">
    {% for post in site.categories.research %}
      <li>
	    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h3>
          <a class="post-link" href="{{ post.url }}#lang=zh">
		    {%- if post.title_zh -%}
			  {{ post.title_zh | escape }}
		    {%- else -%}
			  {{ post.title | escape }}
		    {%- endif -%}
          </a>
        </h3>
      </li>
    {% endfor %}
  </ul>
</div>
