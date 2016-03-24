---
layout: 	post
title: 		"为个人博客添加多说评论框"
date:		2016-03-24
share:      
---


#### 博客已经搭建的差不多了，最后一步就是为其添加上社交功能，现有的一些评论系统可以作为很好的解决方案，笔者最初的愿望是使用国外的Disqus，但是由于只支持国外的社交账号就行第三方登录（大家都懂的），最终还是退而求其次使用了国内的[多说](http://duoshuo.com/)，类似的评论托管系统还有搜狐畅言，友言等。我们应该充分的想象这些系统的完善性（当然不一定是安全的），毕竟使用一段代码就可以拥有靓丽的评论框，不用考虑数据库，评论过滤，统计分析这些繁杂的事务，多么愉快。

<!-- break -->


##### **1**. 去[官网](http://duoshuo.com)上注册一个多说账号，嫌麻烦的可以选择第三方登录
![多说官网图片](http://ww3.sinaimg.cn/mw690/da914f1fgw1f27zx038u1j20qj0n7jyb.jpg)

##### **2**. 注册登录之后添加一个新的站点，按实际情况填写就可以了（没有自己的域名也是木有问题的），注意这里的`多说域名`跟自己博客的域名完全没有关联按照个人喜好填写就可以了，确认无误后点击创建。
![多说建立新站点](http://ww3.sinaimg.cn/mw690/da914f1fgw1f27zwyf3tcj20hy0g1418.jpg)

##### **3**. 创建完成后进入后台管理，选择`工具->获取代码->通用代码`复制页面中的html代码修改之后添加到自己的网页中就可以了，笔者使用的是jekyll博客系统，修改代码中的`data-thred-key`，`data-title`，`data-url`，之后粘贴到_layouts目录下的post.html文件中就可以，多说原生支持了一些博客系统，至于笔者这种不被支持的就只有写原生通用代码了，也是比较方便的。
![后台管理](http://ww1.sinaimg.cn/mw690/da914f1fgw1f27zwz76d1j20mk0h60xw.jpg)

```html
<!-- 多说评论框 start -->
<div class="ds-thread" data-thread-key="请将此处替换成文章在你的站点中的ID" data-title="请替换成文章的标题" data-url="请替换成文章的网址"></div>
<!-- 多说评论框 end -->
<!-- 多说公共JS代码 start (一个网页只需插入一次) -->
<script type="text/javascript">
var duoshuoQuery = {short_name:"mangonob"};
(function() {
var ds = document.createElement('script');
ds.type = 'text/javascript';ds.async = true;
ds.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') + '//static.duoshuo.com/embed.js';
ds.charset = 'UTF-8';
(document.getElementsByTagName('head')[0] 
|| document.getElementsByTagName('body')[0]).appendChild(ds);
})();
</script>
<!-- 多说公共JS代码 end -->
```

##### **4**. 看看效果，还是尽如人意的。
![效果图](http://ww4.sinaimg.cn/mw690/da914f1fgw1f280fkximaj20le0b7754.jpg)

##### **5**. 除了评论框，多说还可以添加社交分享悬浮框，热门评论等功能，喜欢的玩家可以自己探索。本次教程完～

