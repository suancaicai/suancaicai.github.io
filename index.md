---
layout: default
---

<body>
  <div class="index-wrapper">
    <div class="aside">
      <div class="info-card">
        <h1>Yu MingMing</h1>
        <a href="https://weibo.com/u/5204028195?topnav=1&wvr=6&topsug=1&is_all=1" target="_blank"><img src="http://www.weibo.com/favicon.ico" alt="" width="25"/></a>
        <a href="https://www.jianshu.com/u/8fae99b44ef0" target="_blank"><img src="http://www.jianshu.com/favicon.ico" alt="" width="22"/></a>
         <a href="https://github.com/suancaicai" target="_blank"><img src="http://github.com/favicon.ico" alt="" width="22"/></a>
      </div>
      <div id="particles-js"></div>
    </div>

    <div class="index-content">
      <ul class="artical-list">
        {% for post in site.categories.blog %}
        <li>
          <a href="{{ post.url }}" class="title">{{ post.title }}</a>
          <div class="title-desc">{{ post.description }}</div>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
</body>
