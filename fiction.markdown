---
category: fiction
title_en: Fiction
title_zh: 漫剧
layout: page
permalink: "/fiction/"
---

<div class="lang-content" id="en">
  <h2 class="post-list-heading">
	<a href="/">All</a>
	| Fiction
	| <a href="/politics/">Politics</a>
	| <a href="/research/">Research</a>
  </h2>
  <ul class="post-list">
    {% for post in site.categories.fiction %}
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
	| 漫剧
	| <a href="/politics/#lang=zh">政论</a>
	| <a href="/research/#lang=zh">论文</a>
  </h2>
  <ul class="post-list">
    {% for post in site.categories.fiction %}
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
