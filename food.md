---
title: Waipuna - 食道楽
---
### <img src="assets/images/face.png" height="60"> 金欠でも喰道楽

**日頃はダイエットなので、たまには美味しいものが食べたい。**

少ないお小遣いを最大限に活用して、美味しいものを堪能する技を磨き中。後から思い出して、日々のダイエットのつらさを忘れるための備忘録。

<ul class="nav nav-tabs mb-2">
  <li class="nav-item">
    <a class="nav-link link-dark active" data-bs-toggle="tab" href="#post-date" aria-controls="post-date" aria-selected="true">記事（日付）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#post-area" aria-controls="post-area" aria-selected="false">記事（地域）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#post-food" aria-controls="post-food" aria-selected="false">記事（料理）</a>
  </li>
</ul>
<div class="tab-content">
  <div class="tab-pane fade show active" id="post-date">
    <p class="mb-1">2019年</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% capture year %}{{ post.date | date: "%Y" }}{% endcapture %}
            {% if year == "2019" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-1">2018年</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
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
      {% if category[0] == "食べ歩き" %}
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
      {% if category[0] == "食べ歩き" %}
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

    <p class="mb-0">千葉県千葉市</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "千葉市" %}
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
    <p class="mb-0 ms-2">新橋</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "新橋" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">四谷</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "四谷" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">有楽町</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "有楽町" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">品川</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "品川" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">浜松町</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "浜松町" %}
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
      {% if category[0] == "食べ歩き" %}
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

    <p class="mb-0">京都府</p>
    <p class="mb-0 ms-2">京都市</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "京都市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">宇治市</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "宇治市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">大阪府</p>
    <p class="mb-0 ms-2">大阪市本町</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "本町" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">大阪市淀屋橋</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "淀屋橋" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">大阪市中之島</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "中之島" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">門真市</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "門真市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">高槻市</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "高槻市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ms-2">泉佐野市</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "泉佐野市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">香川県小豆島</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "小豆島" %}
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
      {% if category[0] == "食べ歩き" %}
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

    <p class="mb-0">その他</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "その他" %}
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
  <div class="tab-pane fade" id="post-food">
    <p class="mb-0">ラーメン</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "ラーメン" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">そば</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "そば" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">うどん</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "うどん" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">皿うどん</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "皿うどん" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">カレー</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "カレー" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">ステーキ</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "ステーキ" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">おでん</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "おでん" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">定食</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "定食" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">その他</p>
    {% for category in site.categories %}
      {% if category[0] == "食べ歩き" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "その他" %}
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
</div>
