---
layout: default
title: Meet-O-Matic guides
---

{% assign top_post = site.posts[0] %}
{% assign author = site.data.people[top_post.author] %}

<header class="post-header">
  <h2 class="post-title"><a href="{{ top_post.url }}">{{ top_post.title }}</a></h2>
  <div class="post-attribution">
    <img class="post-avatar" alt="{{ author.name }}&#x27;s avatar" height="48" width="48" src="{{ author.avatar }}">
    <p class="post-meta text-muted">
      <time datetime="{{ page.date | date_to_xmlschema }}">
        {%- assign date_format = "%b %-d, %Y" -%}
        {{ page.date | date: date_format }}
      </time>

        • <span class="post-author">
      {%- if author.url -%}
        <a href='{{ author.url }}'>{{ author.name }}</a>
      {%- else -%}
        {{ author.name }}
      {%- endif -%}
        </span>
        on {{ top_post.date | date_to_string }}
    </p>
  </div>
</header>

<hr>

# Meet-O-Matic guides

## Guides

[Getting started](/guides/quick-start) — A quick start guide to using Meet-O-Matic

[Multi-user accounts](/guides/multi-user-accounts) — A guide to Meet-O-Matic’s multiple user accounts

[Clock mode](/guides/clock-mode) — How to use clock mode

[Appointment mode](/guides/appointment-mode) – How to use appointment mode

## Videos

[Scheduling a basic meeting](https://youtu.be/A76tZQUCfFc) — 1 minute video especially for new users

[Tips & Tricks](https://youtu.be/W0oANsIUjzY) — 1 minute video about making Meet-O-Matic even easier!

[Clock Mode 1](https://youtu.be/G5I0l4LGtNU) – Setting meeting times quickly with Meet-O-Matic Pro

[Clock Mode 2](https://youtu.be/jkkFUmyT0nA) – How to set repeating time slots with Meet-O-Matic Pro

[VIP function](https://youtu.be/RBggZ8H3jqI) – For when someone absolutely has to be at your meeting

[All videos](https://www.youtube.com/channel/UC7SbLn88h8JPau6MQZUBWeQ) — Meet-O-Matic’s channel on YouTube
