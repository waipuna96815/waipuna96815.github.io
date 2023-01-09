---
title: Waipuna - テック
---
### <img src="assets/images/face.png" height="60"> テック系よもやま話

**そもそもテック系の厳密な意味を分かっていないが、なんとなく含まれそうな雑多な話**

OSやアプリ、プログラミングのtips、アップル製品を中心とした購入レビューなど（他の人にはあんまり役に立ちそうもないけど）自分としは覚えておきたいあれこれ。

<ul class="nav nav-tabs mb-2">
  <li class="nav-item">
    <a class="nav-link link-dark active" data-bs-toggle="tab" href="#post-date" aria-controls="post-date" aria-selected="false">記事</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#podcast" aria-controls="podcast" aria-selected="false">Podcast</a>
  </li>
  <li class="nav-item">
    <a class="nav-link link-dark" data-bs-toggle="tab" href="#youtube" aria-controls="youtube" aria-selected="false">Youtube</a>
  </li>
</ul>
<div class="tab-content">
  <div class="tab-pane fade show active" id="post-date">
    <p class="mb-1">2017年</p>
    {% for category in site.categories %}
      {% if category[0] == "テック" %}
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
  <div class="tab-pane fade" id="podcast">
    <ul class="list-unstyled ms-3">
      <li>
        <a href="https://podcasts.apple.com/jp/podcast/apple-news-radio-%E3%83%AF%E3%83%B3%E3%83%9C%E3%82%BF%E3%83%B3%E3%81%AE%E5%A3%B0/id346500040">Apple News Radio ワンボタンの声</a>
        （紹介記事は<a href="/posts/20170427a.html">こちら</a>）
      </li>
      <li>
        <a href="https://podcasts.apple.com/jp/podcast/rebuild/id603013428">Rebuild</a>
        （紹介記事は<a href="/posts/20170514a.html">こちら</a>）
      </li>
    </ul>
  </div>
  <div class="tab-pane fade" id="youtube">
    <p class="ms-3">Coming soon</p>
  </div>
</div>
