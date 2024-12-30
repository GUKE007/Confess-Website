# 孤客
# 效果图
![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/dc73a593d5689ce3e4f245d17cf85a10.png)

# 部分代码

```html
<!DOCTYPE html>
<html lang="zh-CN">
<!--版权归孤独 -->
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge, chrome=1">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>孤客</title>
    <meta name="keywords" content="孤独导航、网址大全、网址导航、免费收录、网址大全">
    <meta name="description" content="孤独导航网,为用户提供一站式优质服务,优化用户体验,收录各大平台网站,免费收录各类网站,打造最与众不同的站点导航,导航站点分类齐全,拥有独特的分类栏目,欢迎各大平台合作支持!">
    <!--孤客工作室 -->
    <link rel='stylesheet' id='iconfont-css' href='static/css/iconfont.css' type='text/css' media='all'>
    <link rel='stylesheet' id='bootstrap-css' href='static/css/bootstrap.min.css' type='text/css' media='all'>
    <link rel='stylesheet' id='style-css' href='static/css/style.min.css' type='text/css' media='all'>
    <script src='static/js/jquery.min.js' id='jquery-js'></script>
	<style>

    .bg {
        background-image: url('./static/image/1.jpg')
    }

    </style>
</head>
<body class="user-bookmark-body bookmark-default">
<div id="loading">
    <div id="preloader_3"></div>
</div>
<div class="page-container">
    <div class="bookmark-bg">
        <div class="img-bg bg" id="img-bg"></div>
        <div class="gradient-linear"></div>
    </div>
    <header class="navbar navbar-dark fixed-top">
        <div class="weather">
            <div id="he-plugin-simple" style="display: contents;"></div>
            <script>
                WIDGET = {
                    "CONFIG": {
                        "modules": "02",
                        "background": "5",
                        "tmpColor": "FFFFFF",
                        "tmpSize": "20",
                        "cityColor": "FFFFFF",
                        "citySize": "16",
                        "aqiColor": "FFFFFF",
                        "aqiSize": "16",
                        "weatherIconSize": "30",
                        "alertIconSize": "18",
                        "padding": "0px 5px 0px 5px",
                        "shadow": "0",
                        "language": "auto",
                        "fixed": "false",
                        "vertical": "top",
                        "horizontal": "left",
                        "key": "257fe54e3a0b4cd29b399d2831bd56e0"
                    }
                }
            </script>
            <script src="https://widget.qweather.net/simple/static/js/he-simple-common.js?v=2.0" defer=""></script>
        </div>
    </header>
    <div class="header-big mb-4">
        <div class="s-search">
            <div id="search" class="s-search mx-auto">
                <div class="big-title text-center mb-3 mb-md-5 mt-2">
                    <p class="h1" style="letter-spacing: 6px;">孤客技术导航</p>
                </div>
                <div id="search-list-menu" class="hide-type-list">
                    <div class="s-type text-center overflow-x-auto">
                        <div class="s-type-list big">
                            <div class="anchor" style="position: absolute; left: 50%; opacity: 0;"></div>
                            <label for="type-baidu1" class="active" data-id="group-b"><span>搜索</span></label>
                            <label for="type-br" data-id="group-c"><span>工具</span></label>
                            <label for="type-zhihu" for="type-taobao1" data-id="group-e"><span>生活</span></label>
                            <label for="type-zhaopin" data-id="group-f"><span>求职</span></label>
                        </div>
                    </div>
                </div>
                <form action="/search.html?key=" method="get" target="_blank" class="super-search-fm">
                    <input type="text" id="search-text" class="form-control smart-tips search-key" zhannei="" placeholder="输入关键字搜索" style="outline:0" autocomplete="off">
                    <button type="submit"><i class="iconfont icon-search"></i></button>
                </form>
                <div id="search-list" class="hide-type-list">
                    <div class="search-group group-b s-current">
                        <ul class="search-type">
                            <li><input checked="checked" hidden="" type="radio" name="type" id="type-baidu1" value="https://www.baidu.com/s?wd=" data-placeholder="百度一下"><label for="type-baidu1"><span class="text-muted">百度</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-google1" value="https://www.google.com/search?q=" data-placeholder="谷歌两下"><label for="type-google1"><span class="text-muted">Google</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-360" value="https://www.so.com/s?q=" data-placeholder="360好搜"><label for="type-360"><span class="text-muted">360</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-sogo" value="https://www.sogou.com/web?query=" data-placeholder="搜狗搜索"><label for="type-sogo"><span class="text-muted">搜狗</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-bing1" value="https://cn.bing.com/search?q=" data-placeholder="微软Bing搜索"><label for="type-bing1"><span class="text-muted">Bing</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-sm" value="https://yz.m.sm.cn/s?q=" data-placeholder="UC移动端搜索"><label for="type-sm"><span class="text-muted">神马</span></label></li>
                        </ul>
                    </div>
                    <div class="search-group group-c ">
                        <ul class="search-type">
                            <li><input hidden="" type="radio" name="type" id="type-br" value="https://rank.chinaz.com/all/" data-placeholder="请输入网址(不带https://)"><label for="type-br"><span class="text-muted">权重查询</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-links" value="https://link.chinaz.com/" data-placeholder="请输入网址(不带https://)"><label for="type-links"><span class="text-muted">友链检测</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-icp" value="https://icp.aizhan.com/" data-placeholder="请输入网址(不带https://)"><label for="type-icp"><span class="text-muted">备案查询</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-ping" value="https://ping.chinaz.com/" data-placeholder="请输入网址(不带https://)"><label for="type-ping"><span class="text-muted">PING检测</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-404" value="https://tool.chinaz.com/Links/?DAddress=" data-placeholder="请输入网址(不带https://)"><label for="type-404"><span class="text-muted">死链检测</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-ciku" value="https://www.ciku5.com/s?wd=" data-placeholder="请输入关键词"><label for="type-ciku"><span class="text-muted">关键词挖掘</span></label></li>
                        </ul>
                    </div>
                    <div class="search-group group-d ">
                        <ul class="search-type">
                            <li><input hidden="" type="radio" name="type" id="type-zhihu" value="https://www.zhihu.com/search?type=content&q=" data-placeholder="知乎"><label for="type-zhihu"><span class="text-muted">知乎</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-wechat" value="https://weixin.sogou.com/weixin?type=2&query=" data-placeholder="微信"><label for="type-wechat"><span class="text-muted">微信</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-weibo" value="https://s.weibo.com/weibo/" data-placeholder="微博"><label for="type-weibo"><span class="text-muted">微博</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-douban" value="https://www.douban.com/search?q=" data-placeholder="豆瓣"><label for="type-douban"><span class="text-muted">豆瓣</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-why" value="https://ask.seowhy.com/search/?q=" data-placeholder="SEO问答社区"><label for="type-why"><span class="text-muted">搜外问答</span></label></li>
                        </ul>
                    </div>
                    <div class="search-group group-e ">
                        <ul class="search-type">
                            <li><input hidden="" type="radio" name="type" id="type-taobao1" value="https://s.taobao.com/search?q=" data-placeholder="淘宝"><label for="type-taobao1"><span class="text-muted">淘宝</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-jd" value="https://search.jd.com/Search?keyword=" data-placeholder="京东"><label for="type-jd"><span class="text-muted">京东</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-xiachufang" value="https://www.xiachufang.com/search/?keyword=" data-placeholder="下厨房"><label for="type-xiachufang"><span class="text-muted">下厨房</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-xiangha" value="https://www.xiangha.com/so/?q=caipu&s=" data-placeholder="香哈菜谱"><label for="type-xiangha"><span class="text-muted">香哈菜谱</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-12306" value="https://www.12306.cn/?" data-placeholder="12306"><label for="type-12306"><span class="text-muted">12306</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-kd100" value="https://www.kuaidi100.com/?" data-placeholder="快递100"><label for="type-kd100"><span class="text-muted">快递100</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-qunar" value="https://www.qunar.com/?" data-placeholder="去哪儿"><label for="type-qunar"><span class="text-muted">去哪儿</span></label></li>
                        </ul>
                    </div>
                    <div class="search-group group-f ">
                        <ul class="search-type">
						<li><input hidden="" type="radio" name="type" id="type-liepin" value="https://www.liepin.com/zhaopin/?key=" data-placeholder="猎聘网"><label for="type-liepin"><span class="text-muted">猎聘网</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-zhaopin" value="http://ym.qqmu.com/?key=" data-placeholder="域名抢注"><label for="type-zhaopin"><span class="text-muted">域名抢注</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-51job" value="https://www.qqmu.com/?s=" data-placeholder="QQ沐编程"><label for="type-51job"><span class="text-muted">QQ沐编程</span></label></li>
                            <li><input hidden="" type="radio" name="type" id="type-lagou" value="https://tool.qqmu.com/?s=" data-placeholder="在线工具箱"><label for="type-lagou"><span class="text-muted">在线工具箱</span></label></li>
                            
                        </ul>
                    </div>
                </div>
                <div class="card search-smart-tips" style="display: none">
                    <ul></ul>
                </div>
            </div>
        </div>
    </div>
    <footer class="main-footer footer-type-1 position-relative text-xs">
        <div id="footer-tools" class="d-flex flex-column">
            <a href="javascript:" id="go-to-up" class="btn rounded-circle go-up m-1" rel="go-top">
                <i class="iconfont icon-to-up"></i>
            </a>
            <a href="https://www.vip616.cn" class="btn rounded-circle m-1" data-toggle="tooltip" data-placement="left" title="首页" target="_blank">
                <i class="iconfont icon-home"></i>
            </a>
        </div>
        <div class="footer-inner text-center text-light my-3">
            <div class="footer-text">
                Copyright © 2024 <a href="https://www.vip616.cn"><strong>孤客工作室</strong></a>
            </div>
        </div>
    </footer>
</div>
<script src="static/js/bing.js"></script>
<script src="static/js/popper.min.js"></script>
<script src='static/js/bootstrap.min.js' id='bootstrap-js'></script>
<script src="static/js/theia-sticky-sidebar.js"></script>
<script src='static/js/lazyload.min.js' id='lazyload-js'></script>
<script src='static/js/app.min.js' id='appjs-js'></script>
<script>
    $(document).ready(function () {
        var siteWelcome = $('#loading');
        siteWelcome.addClass('close');
        setTimeout(function () {
            siteWelcome.remove();
        }, 600);
    });
</script>
</body>
</html>
```

# 领取源码
源码完全免费，可以放心使用！可以点一下star嘛~~
# 下期更新预报
> <font color =red>二次元自适应动态引导页</font>
- 📢博客主页：[孤客官方账号](https://github.com/GUKE007)
 - 📢欢迎点赞👍收藏⭐️留言 📝如有错误敬请指正！
 - 📢本文由孤客原创，若侵权联系作者，首发于CSDN博客
 - 📢停下休息的时候不要忘了别人还在奔跑，希望大家抓紧时间学习，全力奔赴更好的生活💻
