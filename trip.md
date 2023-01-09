---
title: Waipuna - 旅行
---
### <img src="assets/images/face.png" height="60"> 出張も気分を換えれば旅日記

**新幹線はヒマ、飛行機は怖い！ でも乗らなくちゃいけないなら、その分楽しもう！！**

知らない街を旅するのは楽しいが、そこへ行くまでの移動は楽しめないタイプ。せっかく行ったのだから、忙しい日常をちょっと忘れる思い出を残そう。

<ul class="nav nav-tabs mb-2">
  <li class="nav-item">
    <a class="nav-link link-dark active" data-bs-toggle="tab" href="#post-date" aria-controls="post-date" aria-selected="true">記事（日付）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#post-area" aria-controls="post-area" aria-selected="false">記事（地域）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#podcast" aria-controls="podcast" aria-selected="false">Podcast</a>
  </li>
</ul>
<div class="tab-content">
  <div class="tab-pane fade show active" id="post-date">
    <p class="mb-1">2018年</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% capture year %}{{ post.date | date: "%Y" }}{% endcapture %}
            {% if year == "2018" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-1">2017年</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% capture year %}{{ post.date | date: "%Y" }}{% endcapture %}
            {% if year == "2017" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}
  </div>
  <div class="tab-pane fade" id="post-area">
    <p class="mb-0">宮城県仙台市</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "仙台市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">東京都</p>
    <p class="mb-0 ms-2">五反田</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "五反田" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">羽田空港</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "羽田空港" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">愛媛県松山市</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "松山市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">マルタ</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "マルタ" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}
  </div>
  <div class="tab-pane fade" id="podcast">
    <p class="ms-3">Coming soon</p>
  </div>
</div>
