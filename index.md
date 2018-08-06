---
layout: default
---

<body>

<div class="index-wrapper">

  <a href="https://github.com/suancaicai"><img style="position: absolute; top: 0; right: 0; border: 0;" src="https://s3.amazonaws.com/github/ribbons/forkme_right_orange_ff7600.png" alt="Fork me on GitHub"></a>


  <!-- 左侧内容 -->
  <div class="aside">

    <div class="info-card">




      <!-- 个人信息 -->
      <div class="site-author motion-element" itemprop="author" itemscope="" itemtype="http://schema.org/Person">
          <img class="site-author-image" itemprop="image" src="/images/image.png" alt="YuMingMing" />
          <p class="site-author-name" itemprop="name">YuMingMing</p>
          <p class="site-description motion-element" itemprop="description">一个iOS小白的技术积累<br />一个对编程充满热爱的iOS开发工程师<br />一个对新技术充满好奇的求知者</p>
      </div>
      <div class="links-of-author motion-element">
          <span class="links-of-author-item">
              <a href="https://weibo.com/u/5204028195?topnav=1&amp;wvr=6&amp;topsug=1&amp;is_all=1" target="_blank" title="weibo">
              <img src="http://www.weibo.com/favicon.ico" alt="" width="22" /> weibo </a>
          </span>

          <span class="links-of-author-item">
            <a href="https://www.jianshu.com/u/8fae99b44ef0" target="_blank" title="jianshu">
            <img src="http://www.jianshu.com/favicon.ico" alt="" width="22" />jianshu</a>
          </span>
          <span class="links-of-author-item">
              <a href="https://github.com/suancaicai" target="_blank" title="GitHub">
              <img src="http://github.com/favicon.ico" alt="" width="22" />GitHub</a>
          </span>
      </div>



      <!-- <nav class="site-nav">

          <ul id="menu" class="menu">
              <li class="menu-item menu-item-home">
                <a href="/" rel="section"><i class="menu-item-icon fa fa-fw fa-home"></i> <br />首页</a>
              </li>
              <li class="menu-item menu-item-categories">
                <a href="/categories/" rel="section"><i class="menu-item-icon fa fa-fw fa-th"></i> <br />分类</a>
              </li>
              <li class="menu-item menu-item-archives">
                <a href="/archives/" rel="section"><i class="menu-item-icon fa fa-fw fa-archive"></i> <br />目录</a>
              </li>
              <li class="menu-item menu-item-tags">
                <a href="/tags/" rel="section"><i class="menu-item-icon fa fa-fw fa-tags"></i> <br />标签</a>
              </li>
              <li class="menu-item menu-item-about">
                <a href="/about/" rel="section"><i class="menu-item-icon fa fa-fw fa-user"></i> <br />关于</a>
              </li>
              <li class="menu-item menu-item-search">
                  <a href="javascript:;" class="popup-trigger"><i class="menu-item-icon fa fa-search fa-fw"></i> <br />搜索  </a>
              </li>
          </ul>

          <div class="site-search">
                <div class="popup search-popup local-search-popup">
                <div class="local-search-header clearfix">
                  <span class="search-icon"><i class="fa fa-search"></i></span>
                  <span class="popup-btn-close"><i class="fa fa-times-circle"></i></span>
                  <div class="local-search-input-wrapper">
                    <input autocomplete="off" placeholder="搜索..."   spellcheck="false" type="text"  id="local-search-input">
                  </div>
                </div>
                <div id="local-search-result"></div>
              </div>
          </div>
      </nav> -->


    </div>

    <!-- 左侧背景色 -->
    <div id="particles-js"></div>  
  </div>


  <!-- 右边内容 -->
  <div class="index-content">


          <!-- 文章列表 -->
            <ul class="artical-list">
              {% for post in site.categories.blog %}
              <li>
                <a href="{{ post.url }}" class="title">{{ post.title }}</a>
                <div class="title-desc">{{ post.description }}</div>
              </li>
              {% endfor %}
            </ul>




            <!-- 分页 -->
            <!-- <div id="content" class="content">
                <nav class="pagination">
                  <span class="page-number current">1</span>
                  <a class="page-number" href="/page/2/">2</a>
                  <a class="extend next" rel="next" href="/page/2/"><i class="fa fa-angle-right"></i></a>
                </nav>
            </div> -->


            <!-- 底部内容 -->
            <!-- <footer id="footer" class="footer">
              <div class="footer-inner">
                  <div class="copyright">
                      <span class="with-love">
                          <i class="fa fa-user"></i>
                      </span>
                      <span class="author" itemprop="copyrightHolder">YuMingMing</span>
                      &copy;
                      <span itemprop="copyrightYear">2018-08-01</span>
                      <span class="post-meta-divider">|</span>
                      <span class="post-meta-item-icon">
                        <i class="fa fa-area-chart"></i>
                      </span>
                      <span class="post-meta-item-text">博客总字数&#58;</span>
                      <span title="博客总字数">7.1k</span>
                  </div>

                  <div class="theme-info">
                      <span>　<i class="fa fa-bomb"></i></span>
                      <span id="showDays"></span>
                  </div>
                  <br/>
                     本页点击 <span id="busuanzi_value_page_pv"></span> 次
                    |  本站总点击 <span id="busuanzi_value_site_pv"></span> 次
                    |  您是第 <span id="busuanzi_value_site_uv"></span> 位访客
                   <br/>
                    <a href="http://www.miitbeian.gov.cn/">浙ICP备18014749号</a>

                  <script async src="https://dn-lbstatics.qbox.me/busuanzi/2.3/busuanzi.pure.mini.js">
                  </script>
                  <script>
                    var seconds = 1000;
                    var minutes = seconds * 60;
                    var hours = minutes * 60;
                    var days = hours * 24;
                    var years = days * 365;
                    var birthDay = Date.UTC(2018,03,30,00,00,00); // 这里设置建站时间
                    setInterval(function() {
                      var today = new Date();
                      var todayYear = today.getFullYear();
                      var todayMonth = today.getMonth()+1;
                      var todayDate = today.getDate();
                      var todayHour = today.getHours();
                      var todayMinute = today.getMinutes();
                      var todaySecond = today.getSeconds();
                      var now = Date.UTC(todayYear,todayMonth,todayDate,todayHour,todayMinute,todaySecond);
                      var diff = now - birthDay;
                      var diffYears = Math.floor(diff/years);
                      var diffDays = Math.floor((diff/days)-diffYears*365);
                      var diffHours = Math.floor((diff-(diffYears*365+diffDays)*days)/hours);
                      var diffMinutes = Math.floor((diff-(diffYears*365+diffDays)*days-diffHours*hours)/minutes);
                      var diffSeconds = Math.floor((diff-(diffYears*365+diffDays)*days-diffHours*hours-diffMinutes*minutes)/seconds);
                        document.getElementById('showDays').innerHTML="本站已运行 "+diffYears+" 年 "+diffDays+" 天 "+diffHours+" 小时 "+diffMinutes+" 分钟 "+diffSeconds+" 秒";
                    }, 1000);
                  </script>

                  <script src="//cdn1.lncld.net/static/js/2.5.0/av-min.js"></script>
                  <script>
                      var APP_ID = '8lLHEJN0b5CQM0z0zwINSAKj-gzGzoHsz';
                      var APP_KEY = 'P8FLghl21NYuCyoqdDB0o1WA';
                      AV.init({
                          appId: APP_ID,
                          appKey: APP_KEY
                      });
                      // 显示次数
                      function showTime(Counter) {
                          var query = new AV.Query("Counter");
                          if($(".leancloud_visitors").length > 0){
                              var url = $(".leancloud_visitors").attr('id').trim();
                              // where field
                              query.equalTo("words", url);
                              // count
                              query.count().then(function (number) {
                                  // There are number instances of MyClass where words equals url.
                                  $(document.getElementById(url)).text(number?  number : '--');
                              }, function (error) {
                                  // error is an instance of AVError.
                              });
                          }
                      }
                      // 追加pv
                      function addCount(Counter) {
                          var url = $(".leancloud_visitors").length > 0 ? $(".leancloud_visitors").attr('id').trim() : 'icafebolger.com';
                          var Counter = AV.Object.extend("Counter");
                          var query = new Counter;
                          query.save({
                              words: url
                          }).then(function (object) {
                          })
                      }
                      $(function () {
                          var Counter = AV.Object.extend("Counter");
                          addCount(Counter);
                          showTime(Counter);
                      });
                  </script>

              </div>
            </footer>


            <div class="back-to-top">
              <i class="fa fa-arrow-up"></i>  
            </div> -->

  </div>




</div>





















  <!-- 屏幕动画效果 -->
  <script type="text/javascript" src="/lib/canvas-nest/canvas-nest.min.js"></script>

  <script type="text/javascript">
    if (Object.prototype.toString.call(window.Promise) !== '[object Function]') {
      window.Promise = null;
    }
  </script>


  <link href="/css/main.css?v=5.1.4" rel="stylesheet" type="text/css" />




  <link rel="apple-touch-icon" sizes="180x180" href="/images/ic-fact-180.png?v=5.1.4">
  <link rel="icon" type="image/png" sizes="32x32" href="/images/ic-fact-32.png?v=5.1.4">
  <link rel="icon" type="image/png" sizes="16x16" href="/images/ic-fact-16.png?v=5.1.4">
  <link rel="mask-icon" href="/images/logo.svg?v=5.1.4" color="#222">


  <script type="text/javascript">
    if (Object.prototype.toString.call(window.Promise) !== '[object Function]') {
      window.Promise = null;
    }
  </script>
  <script type="text/javascript" src="/lib/jquery/index.js?v=2.1.3"></script>
  <script type="text/javascript" src="/lib/fastclick/lib/fastclick.min.js?v=1.0.6"></script>
   <script type="text/javascript" src="/lib/jquery_lazyload/jquery.lazyload.js?v=1.9.7"></script>
  <script type="text/javascript" src="/lib/velocity/velocity.min.js?v=1.2.1"></script>
  <script type="text/javascript" src="/lib/velocity/velocity.ui.min.js?v=1.2.1"></script>
   <script type="text/javascript" src="/lib/fancybox/source/jquery.fancybox.pack.js?v=2.1.5"></script>

  <script type="text/javascript" src="/js/src/utils.js?v=5.1.4"></script>
  <script type="text/javascript" src="/js/src/motion.js?v=5.1.4"></script>
  <script type="text/javascript" src="/js/src/affix.js?v=5.1.4"></script>
  <script type="text/javascript" src="/js/src/schemes/pisces.js?v=5.1.4"></script>
  <script type="text/javascript" src="/js/src/bootstrap.js?v=5.1.4"></script>

  <script src="//cdn1.lncld.net/static/js/3.0.4/av-min.js"></script>
  <script src="//unpkg.com/valine/dist/Valine.min.js"></script>


  <!-- 有没有用先放着再说 -->
  <script type="text/javascript">
      var GUEST = ['nick','mail','link'];
      var guest = 'nick,mail,link';
      guest = guest.split(',').filter(item=>{
        return GUEST.indexOf(item)>-1;
      });
      new Valine({
          el: '#comments' ,
          verify: false,
          notify: true,
          appId: '8lLHEJN0b5CQM0z0zwINSAKj-gzGzoHsz',
          appKey: 'P8FLghl21NYuCyoqdDB0o1WA',
          placeholder: '既然来了，那就留下你的足迹吧~',
          avatar:'monsterid',
          guest_info:guest,
          pageSize:'10' || 10,
      });
  </script>
  <script type="text/javascript">
    // Popup Window;
    var isfetched = false;
    var isXml = true;
    // Search DB path;
    var search_path = "search.xml";
    if (search_path.length === 0) {
      search_path = "search.xml";
    } else if (/json$/i.test(search_path)) {
      isXml = false;
    }
    var path = "/" + search_path;
    // monitor main search box;

    var onPopupClose = function (e) {
      $('.popup').hide();
      $('#local-search-input').val('');
      $('.search-result-list').remove();
      $('#no-result').remove();
      $(".local-search-pop-overlay").remove();
      $('body').css('overflow', '');
    }

    function proceedsearch() {
      $("body")
        .append('<div class="search-popup-overlay local-search-pop-overlay"></div>')
        .css('overflow', 'hidden');
      $('.search-popup-overlay').click(onPopupClose);
      $('.popup').toggle();
      var $localSearchInput = $('#local-search-input');
      $localSearchInput.attr("autocapitalize", "none");
      $localSearchInput.attr("autocorrect", "off");
      $localSearchInput.focus();
    }

    // search function;
    var searchFunc = function(path, search_id, content_id) {
      'use strict';

      // start loading animation
      $("body")
        .append('<div class="search-popup-overlay local-search-pop-overlay">' +
          '<div id="search-loading-icon">' +
          '<i class="fa fa-spinner fa-pulse fa-5x fa-fw"></i>' +
          '</div>' +
          '</div>')
        .css('overflow', 'hidden');
      $("#search-loading-icon").css('margin', '20% auto 0 auto').css('text-align', 'center');

      $.ajax({
        url: path,
        dataType: isXml ? "xml" : "json",
        async: true,
        success: function(res) {
          // get the contents from search data
          isfetched = true;
          $('.popup').detach().appendTo('.header-inner');
          var datas = isXml ? $("entry", res).map(function() {
            return {
              title: $("title", this).text(),
              content: $("content",this).text(),
              url: $("url" , this).text()
            };
          }).get() : res;
          var input = document.getElementById(search_id);
          var resultContent = document.getElementById(content_id);
          var inputEventFunction = function() {
            var searchText = input.value.trim().toLowerCase();
            var keywords = searchText.split(/[\s\-]+/);
            if (keywords.length > 1) {
              keywords.push(searchText);
            }
            var resultItems = [];
            if (searchText.length > 0) {
              // perform local searching
              datas.forEach(function(data) {
                var isMatch = false;
                var hitCount = 0;
                var searchTextCount = 0;
                var title = data.title.trim();
                var titleInLowerCase = title.toLowerCase();
                var content = data.content.trim().replace(/<[^>]+>/g,"");
                var contentInLowerCase = content.toLowerCase();
                var articleUrl = decodeURIComponent(data.url);
                var indexOfTitle = [];
                var indexOfContent = [];
                // only match articles with not empty titles
                if(title != '') {
                  keywords.forEach(function(keyword) {
                    function getIndexByWord(word, text, caseSensitive) {
                      var wordLen = word.length;
                      if (wordLen === 0) {
                        return [];
                      }
                      var startPosition = 0, position = [], index = [];
                      if (!caseSensitive) {
                        text = text.toLowerCase();
                        word = word.toLowerCase();
                      }
                      while ((position = text.indexOf(word, startPosition)) > -1) {
                        index.push({position: position, word: word});
                        startPosition = position + wordLen;
                      }
                      return index;
                    }

                    indexOfTitle = indexOfTitle.concat(getIndexByWord(keyword, titleInLowerCase, false));
                    indexOfContent = indexOfContent.concat(getIndexByWord(keyword, contentInLowerCase, false));
                  });
                  if (indexOfTitle.length > 0 || indexOfContent.length > 0) {
                    isMatch = true;
                    hitCount = indexOfTitle.length + indexOfContent.length;
                  }
                }

                // show search results

                if (isMatch) {
                  // sort index by position of keyword

                  [indexOfTitle, indexOfContent].forEach(function (index) {
                    index.sort(function (itemLeft, itemRight) {
                      if (itemRight.position !== itemLeft.position) {
                        return itemRight.position - itemLeft.position;
                      } else {
                        return itemLeft.word.length - itemRight.word.length;
                      }
                    });
                  });

                  // merge hits into slices

                  function mergeIntoSlice(text, start, end, index) {
                    var item = index[index.length - 1];
                    var position = item.position;
                    var word = item.word;
                    var hits = [];
                    var searchTextCountInSlice = 0;
                    while (position + word.length <= end && index.length != 0) {
                      if (word === searchText) {
                        searchTextCountInSlice++;
                      }
                      hits.push({position: position, length: word.length});
                      var wordEnd = position + word.length;

                      // move to next position of hit

                      index.pop();
                      while (index.length != 0) {
                        item = index[index.length - 1];
                        position = item.position;
                        word = item.word;
                        if (wordEnd > position) {
                          index.pop();
                        } else {
                          break;
                        }
                      }
                    }
                    searchTextCount += searchTextCountInSlice;
                    return {
                      hits: hits,
                      start: start,
                      end: end,
                      searchTextCount: searchTextCountInSlice
                    };
                  }

                  var slicesOfTitle = [];
                  if (indexOfTitle.length != 0) {
                    slicesOfTitle.push(mergeIntoSlice(title, 0, title.length, indexOfTitle));
                  }

                  var slicesOfContent = [];
                  while (indexOfContent.length != 0) {
                    var item = indexOfContent[indexOfContent.length - 1];
                    var position = item.position;
                    var word = item.word;
                    // cut out 100 characters
                    var start = position - 20;
                    var end = position + 80;
                    if(start < 0){
                      start = 0;
                    }
                    if (end < position + word.length) {
                      end = position + word.length;
                    }
                    if(end > content.length){
                      end = content.length;
                    }
                    slicesOfContent.push(mergeIntoSlice(content, start, end, indexOfContent));
                  }

                  // sort slices in content by search text's count and hits' count

                  slicesOfContent.sort(function (sliceLeft, sliceRight) {
                    if (sliceLeft.searchTextCount !== sliceRight.searchTextCount) {
                      return sliceRight.searchTextCount - sliceLeft.searchTextCount;
                    } else if (sliceLeft.hits.length !== sliceRight.hits.length) {
                      return sliceRight.hits.length - sliceLeft.hits.length;
                    } else {
                      return sliceLeft.start - sliceRight.start;
                    }
                  });

                  // select top N slices in content

                  var upperBound = parseInt('1');
                  if (upperBound >= 0) {
                    slicesOfContent = slicesOfContent.slice(0, upperBound);
                  }

                  // highlight title and content

                  function highlightKeyword(text, slice) {
                    var result = '';
                    var prevEnd = slice.start;
                    slice.hits.forEach(function (hit) {
                      result += text.substring(prevEnd, hit.position);
                      var end = hit.position + hit.length;
                      result += '<b class="search-keyword">' + text.substring(hit.position, end) + '</b>';
                      prevEnd = end;
                    });
                    result += text.substring(prevEnd, slice.end);
                    return result;
                  }

                  var resultItem = '';

                  if (slicesOfTitle.length != 0) {
                    resultItem += "<li><a href='" + articleUrl + "' class='search-result-title'>" + highlightKeyword(title, slicesOfTitle[0]) + "</a>";
                  } else {
                    resultItem += "<li><a href='" + articleUrl + "' class='search-result-title'>" + title + "</a>";
                  }

                  slicesOfContent.forEach(function (slice) {
                    resultItem += "<a href='" + articleUrl + "'>" +
                      "<p class=\"search-result\">" + highlightKeyword(content, slice) +
                      "...</p>" + "</a>";
                  });

                  resultItem += "</li>";
                  resultItems.push({
                    item: resultItem,
                    searchTextCount: searchTextCount,
                    hitCount: hitCount,
                    id: resultItems.length
                  });
                }
              })
            };
            if (keywords.length === 1 && keywords[0] === "") {
              resultContent.innerHTML = '<div id="no-result"><i class="fa fa-search fa-5x" /></div>'
            } else if (resultItems.length === 0) {
              resultContent.innerHTML = '<div id="no-result"><i class="fa fa-frown-o fa-5x" /></div>'
            } else {
              resultItems.sort(function (resultLeft, resultRight) {
                if (resultLeft.searchTextCount !== resultRight.searchTextCount) {
                  return resultRight.searchTextCount - resultLeft.searchTextCount;
                } else if (resultLeft.hitCount !== resultRight.hitCount) {
                  return resultRight.hitCount - resultLeft.hitCount;
                } else {
                  return resultRight.id - resultLeft.id;
                }
              });
              var searchResultList = '<ul class=\"search-result-list\">';
              resultItems.forEach(function (result) {
                searchResultList += result.item;
              })
              searchResultList += "</ul>";
              resultContent.innerHTML = searchResultList;
            }
          }

          if ('auto' === 'auto') {
            input.addEventListener('input', inputEventFunction);
          } else {
            $('.search-icon').click(inputEventFunction);
            input.addEventListener('keypress', function (event) {
              if (event.keyCode === 13) {
                inputEventFunction();
              }
            });
          }

          // remove loading animation
          $(".local-search-pop-overlay").remove();
          $('body').css('overflow', '');

          proceedsearch();
        }
      });
    }

    // handle and trigger popup window;
    $('.popup-trigger').click(function(e) {
      e.stopPropagation();
      if (isfetched === false) {
        searchFunc(path, 'local-search-input', 'local-search-result');
      } else {
        proceedsearch();
      };
    });

    $('.popup-btn-close').click(onPopupClose);
    $('.popup').click(function(e){
      e.stopPropagation();
    });
    $(document).on('keyup', function (event) {
      var shouldDismissSearchPopup = event.which === 27 &&
        $('.search-popup').is(':visible');
      if (shouldDismissSearchPopup) {
        onPopupClose();
      }
    });
  </script>
  <script src="https://cdn1.lncld.net/static/js/av-core-mini-0.6.4.js"></script>
  <script>AV.initialize("8lLHEJN0b5CQM0z0zwINSAKj-gzGzoHsz", "P8FLghl21NYuCyoqdDB0o1WA");</script>
  <script>
    function showTime(Counter) {
      var query = new AV.Query(Counter);
      var entries = [];
      var $visitors = $(".leancloud_visitors");

      $visitors.each(function () {
        entries.push( $(this).attr("id").trim() );
      });

      query.containedIn('url', entries);
      query.find()
        .done(function (results) {
          var COUNT_CONTAINER_REF = '.leancloud-visitors-count';

          if (results.length === 0) {
            $visitors.find(COUNT_CONTAINER_REF).text(0);
            return;
          }

          for (var i = 0; i < results.length; i++) {
            var item = results[i];
            var url = item.get('url');
            var time = item.get('time');
            var element = document.getElementById(url);

            $(element).find(COUNT_CONTAINER_REF).text(time);
          }
          for(var i = 0; i < entries.length; i++) {
            var url = entries[i];
            var element = document.getElementById(url);
            var countSpan = $(element).find(COUNT_CONTAINER_REF);
            if( countSpan.text() == '') {
              countSpan.text(0);
            }
          }
        })
        .fail(function (object, error) {
          console.log("Error: " + error.code + " " + error.message);
        });
    }

    function addCount(Counter) {
      var $visitors = $(".leancloud_visitors");
      var url = $visitors.attr('id').trim();
      var title = $visitors.attr('data-flag-title').trim();
      var query = new AV.Query(Counter);

      query.equalTo("url", url);
      query.find({
        success: function(results) {
          if (results.length > 0) {
            var counter = results[0];
            counter.fetchWhenSave(true);
            counter.increment("time");
            counter.save(null, {
              success: function(counter) {
                var $element = $(document.getElementById(url));
                $element.find('.leancloud-visitors-count').text(counter.get('time'));
              },
              error: function(counter, error) {
                console.log('Failed to save Visitor num, with error message: ' + error.message);
              }
            });
          } else {
            var newcounter = new Counter();
            /* Set ACL */
            var acl = new AV.ACL();
            acl.setPublicReadAccess(true);
            acl.setPublicWriteAccess(true);
            newcounter.setACL(acl);
            /* End Set ACL */
            newcounter.set("title", title);
            newcounter.set("url", url);
            newcounter.set("time", 1);
            newcounter.save(null, {
              success: function(newcounter) {
                var $element = $(document.getElementById(url));
                $element.find('.leancloud-visitors-count').text(newcounter.get('time'));
              },
              error: function(newcounter, error) {
                console.log('Failed to create');
              }
            });
          }
        },
        error: function(error) {
          console.log('Error:' + error.code + " " + error.message);
        }
      });
    }

    $(function() {
      var Counter = AV.Object.extend("Counter");
      if ($('.leancloud_visitors').length == 1) {
        addCount(Counter);
      } else if ($('.post-title-link').length > 1) {
        showTime(Counter);
      }
    });
  </script>
  <script>
    (function(){
        var bp = document.createElement('script');
        var curProtocol = window.location.protocol.split(':')[0];
        if (curProtocol === 'https') {
            bp.src = 'https://zz.bdstatic.com/linksubmit/push.js';
        }
        else {
            bp.src = 'http://push.zhanzhang.baidu.com/push.js';
        }
        var s = document.getElementsByTagName("script")[0];
        s.parentNode.insertBefore(bp, s);
    })();
  </script>





</body>
