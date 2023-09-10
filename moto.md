---
title: Waipuna - バイク
---
### <img src="assets/images/face.png" height="60"> 徒然バイク日記

**金なし、テクなし、根性なし、さらに仲間なしライダーの奮闘記**

バイクやツーリング、グッズなどの話しを徒然なるままに書き残す。

<ul class="nav nav-tabs mb-2">
  <li class="nav-item">
    <a class="nav-link link-dark active" data-bs-toggle="tab" href="#post-date" aria-controls="post-date" aria-selected="true">記事（日付）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#post-touring" aria-controls="post-touring" aria-selected="false">記事（ツーリング）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#motogp" aria-controls="motogp" aria-selected="false">MotoGP</a>
  </li>
</ul>
<div class="tab-content">
  <div class="tab-pane fade show active" id="post-date">

<p class="mb-1">2023年</p>
<ul class="list-unstyled ms-3 mb-1">
<li><a href="pages/moto-2023gp.html">MotoGP：第12戦サンマリノGPの成績を追加</a> （2023年09月10日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第11戦スペイン・カタルーニャGPの成績を追加</a> （2023年09月04日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第9戦イギリスGPと第10戦オーストリアGPの成績を追加</a> （2023年08月28日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第8戦オランダGPの成績を追加</a> （2023年06月25日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第7戦ドイツGPの成績を追加</a> （2023年06月18日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第6戦イタリアGPの成績を追加</a> （2023年06月12日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第5戦フランスGPの成績を追加</a> （2023年05月14日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第4戦スペインGPの成績を追加</a> （2023年04月30日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：第3戦アメリカGPの成績を追加</a> （2023年04月22日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：主な成績</a> （2023年04月09日）</li>
<li><a href="pages/moto-2023gp.html">MotoGP：2023 カレンダー</a> （2023年02月05日）</li>
</ul>

<p class="mb-1">2021年</p>
<ul class="list-unstyled ms-3 mb-1">
<li><a href="pages/moto-byesr.html">さよなら、SR400</a> （2021年08月22日）</li>
<li><a href="pages/moto-hellobmw.html">こんにちは、BMW R1250RT</a> （2021年08月07日）</li>
</ul>

<p class="mb-1">2020年</p>
<ul class="list-unstyled ms-3 mb-1">
<li><a href="pages/moto-HT2020.html">北海道ツーリング 2020</a> （2020年08月23日）</li>
</ul>

    <p class="mb-1">2019年</p>
    {% for category in site.categories %}
      {% if category[0] == "バイク" %}
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
      {% if category[0] == "バイク" %}
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
      {% if category[0] == "バイク" %}
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
  <div class="tab-pane fade" id="post-touring">
<p class="mb-0">北海道</p>
<ul class="list-unstyled ms-3 mb-1">
<li><a href="pages/moto-HT2020.html">北海道ツーリング 2020</a> （2020年08月23日）</li>
</ul>

    <p class="mb-0">近畿</p>
    {% for category in site.categories %}
      {% if category[0] == "バイク" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "ツーリング" %}
              {% if post.tags contains "琵琶湖"
                 or post.tags contains "加太"
                 or post.tags contains "淡路島" %}
                <li>
                  <a href="{{ post.url }}">{{ post.title }}</a>
                  （{{ post.date | date: "%Y年%m月%d日" }}）
                </li>
              {% endif %}
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">四国</p>
    {% for category in site.categories %}
      {% if category[0] == "バイク" %}
        <ul class="list-unstyled ms-3">
          {% for post in category[1] %}
            {% if post.tags contains "ツーリング" %}
              {% if post.tags contains "四国" %}
                <li>
                  <a href="{{ post.url }}">{{ post.title }}</a>
                  （{{ post.date | date: "%Y年%m月%d日" }}）
                </li>
              {% endif %}
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}
  </div>
  <div class="tab-pane fade" id="motogp">
    <ul class="list-unstyled ms-3">
      <li><a href="pages/moto-2023gp.html">2023 MotoGP：主な成績</a> （2023年04月09日）</li>
      <li><a href="pages/moto-2023gp.html">2023 MotoGP：カレンダー</a> （2023年02月05日）</li>
    </ul>
  </div>
</div>
