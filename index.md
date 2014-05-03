---
layout: page
title: RHG Reading Okinawa
---
{% include JB/setup %}

ここは、オンラインで [Ruby Hacking Guide](http://i.loveruby.net/ja/rhg/) 読書会を試してみる成果が投入される所です。

ご興味ある方は [RHG Reading Okinawa](https://github.com/RHGReadingOkinawa/rhgreadingokinawa.github.com) 方面にコンタクトとってみてください。

## Posts

読んだ記録は以下から確認できます。

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

- index.md の refine
