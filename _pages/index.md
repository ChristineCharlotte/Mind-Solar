---
layout: page
title: Mind Solar | 心晖：闪耀每一片灵感
id: home
permalink: /
---

# Welcome! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  一个基于 [[MarkDown]] 和 [[Obsidian]] 的 <span style="font-weight: bold">[[双链信息中心]]</span>。Mind Solar，将心灵比作太阳，让每个想法如阳光般闪耀。
</p>

This digital garden template is free, open-source, and [available on GitHub here](https://github.com/olivla/mind-solar).

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
