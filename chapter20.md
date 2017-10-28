## 一．响应式导航 

```
//基本导航组件+响应式
<nav class="navbar navbar-default navbar-fixed-top">
<div class="container">
<div class="navbar-header">
<a href="#" class="navbar-brand"
style="margin:0;padding:0;"><img src="img/logo.png" alt="瓢城企训网"></a>
<button type="button" class="navbar-toggle"
data-toggle="collapse" data-target="#navbar-collapse">
<span class="sr-only">切换导航</span>
<span class="icon-bar"></span>
<span class="icon-bar"></span>
<span class="icon-bar"></span>
</button>
</div>
<div class="collapse navbar-collapse" id="navbar-collapse">
<ul class="nav navbar-nav navbar-right"
style="margin-top:0;">
<li class="active"><a href="#"><span class="glyphicon
glyphicon-home"></span> 首页</a></li>
<li><a href="#"><span class="glyphicon
glyphicon-list"></span> 资讯</a></li>
<li><a href="#"><span class="glyphicon
glyphicon-fire"></span> 案例</a></li>
<li><a href="#"><span class="glyphicon
glyphicon-question-sign"></span> 关于</a></li>
</ul>
</div>
</div>
</nav>
```

## 二．响应式轮播图 

```
//响应式轮播图
<div id="myCarousel" class="carousel slide">
<ol class="carousel-indicators">
<li data-target="#myCarousel" data-slide-to="0"
class="active"></li>
<li data-target="#myCarousel" data-slide-to="1"></li>
<li data-target="#myCarousel" data-slide-to="2"></li>
</ol>
<div class="carousel-inner">
<div class="item active" style="background:#223240;">
<a href="#"><img src="img/slide1.png" alt="第一张"></a>
</div>
<div class="item" style="background:#F5E4DC;">
<a href="#"><img src="img/slide2.png" alt="第二张"></a>
</div>
<div class="item" style="background:#DE2A2D;">
<a href="#"><img src="img/slide3.png" alt="第三张"></a>
</div>
</div>
<a href="#myCarousel" data-slide="prev" class="carousel-control
left">&lsaquo;</a>
<a href="#myCarousel" data-slide="next" class="carousel-control
right">&rsaquo;</a>
</div>
//所需要的 jQuery 控制
$('#myCarousel').carousel({
//设置自动播放/2 秒
interval : 3000,
});
```

## 三．首页内容介绍[上] 

```
//关于上节课轮播图，手册上其实有一个更好的方案，并不需要通过额外的代码控制。
<a href="#myCarousel" data-slide="prev" class="carousel-control left">
<span class="glyphicon glyphicon-chevron-left"></span>
</a>
<a href="#myCarousel" data-slide="next" class="carousel-control
right">
<span class="glyphicon glyphicon-chevron-right"></span>
</a>
//内容介绍上
<div class="tab1">
<div class="container">
<h2 class="tab-h2">「 为什么选择瓢城企业培训 」</h2>
<p class="tab-p">强大的师资力量，完美的实战型管理课程，让您的企业
实现质的腾飞！</p>
<div class="row">
<div class="col-md-6 col">
<div class="media">
<div class="media-left media-top">
<a href="#">
<img class="media-object"
src="img/tab1-1.png" alt="...">
</a>
</div>
<div class="media-body">
<h4 class="media-heading">课程内容</h4>
<p class="text-muted">其他：高校不知名的讲师编写，
没有任何实战价值的教材！</p>
<p>其他：知名企业家、管理学大师联合编写的具有实现性
教材！</p>
</div>
</div></div>
<div class="col-md-6 col">
<div class="media">
<div class="media-left media-top">
<a href="#">
<img class="media-object"
src="img/tab1-2.png" alt="...">
</a>
</div>
<div class="media-body">
<h4 class="media-heading">师资力量</h4>
<p class="text-muted">其他：非欧美正牌大学毕业的、
业界没有知名度的讲师！</p>
<p>其他：美国哈佛、耶鲁等世界一流高校、享有声誉的名
牌专家！</p>
</div>
</div>
</div>
<div class="col-md-6 col">
<div class="media">
<div class="media-left media-top">
<a href="#">
<img class="media-object"
src="img/tab1-3.png" alt="...">
</a>
</div>
<div class="media-body">
<h4 class="media-heading">课时安排</h4>
<p class="text-muted">其他：无法保证上课效率、没
有时间表，任务无法完成！</p>
<p>其他：保证正常的上课效率、制定一张时间表、当天的
任务当天完成！</p>
</div>
</div>
</div>
<div class="col-md-6 col">
<div class="media">
<div class="media-left media-top">
<a href="#">
<img class="media-object"
src="img/tab1-4.png" alt="...">
</a>
</div>
<div class="media-body"><h4 class="media-heading">服务团队</h4>
<p class="text-muted">其他：社会招聘的、服务水平
参差不齐的普通员工！</p>
<p>其他：内部培养、经受过良好高端服务培训的高标准员
工！</p>
</div>
</div>
</div>
</div>
</div>
</div>
//对应的 CSS 部分
body {
font-family: "Helvetica Neue", Helvetica, Arial, "Microsoft Yahei
UI", "Microsoft YaHei", SimHei, "\5B8B\4F53", simsun, sans-serif;
}
.tab-h2 {
font-size: 20px;
color: #0059B2;
text-align: center;
letter-spacing: 1px;
}
.tab-p {
font-size: 15px;
color: #999;
text-align: center;
letter-spacing: 1px;
margin: 20px 0 40px 0;
}
.tab1 {
margin: 30px 0;
color: #666;
}
.tab1 .media-heading {
margin: 5px 0 20px 0;
}
.tab1 .text-muted {
color: #999;
text-decoration: line-through;
}
.tab1 .media-heading {margin: 5px 0 20px 0;
}
.tab1 .text-muted {
color: #999;
text-decoration: line-through;
}
.tab1 .col {
padding: 20px;
}
/* 小屏幕（平板，大于等于 768px） */
@media (min-width: 768px) {
.tab-h2 {
font-size: 26px;
}
.tab-p {
font-size: 16px;
}
}
/* 中等屏幕（桌面显示器，大于等于 992px） */
@media (min-width: 992px) {
.tab-h2 {
font-size: 28px;
}
.tab-p {
font-size: 17px;
}
}
/* 大屏幕（大桌面显示器，大于等于 1200px） */
@media (min-width: 1200px) {
.tab-h2 {
font-size: 30px;
}
.tab-p {
font-size: 18px;
}
}
```

## 四．首页内容介绍[下] 

```
//先完成底部的 footer
<footer id="footer" class="text-muted">
<div class="container">
<p>企业培训 | 合作事宜 | 版权投诉</p>
<p>苏 ICP 备 12345678. © 2009-2016 瓢城企训网. Powered by
Bootstrap.</p>
</div>
</footer>
//底部 CSS
#footer {
padding: 20px;
text-align: center;
background-color: #eee;
border-top: 1px solid #ccc;
}
//两段内容
<div class="tab2">
<div class="container">
<div class="row">
<div class="col-md-6 col-sm-6 tab2-img">
<img src="img/tab2.png" alt="" class="auto
img-responsive center-block">
</div>
<div class="text col-md-6 col-sm-6 tab2-text">
<h3>强大的学习体系</h3>
<p>经过管理学大师层层把关、让您的企业突飞猛进。</p>
</div>
</div>
</div>
</div><div class="tab3">
<div class="container">
<div class="row">
<div class="col-md-6 col-sm-6">
<img src="img/tab3.png" alt="" class="auto
img-responsive center-block">
</div>
<div class="text col-md-6 col-sm-6">
<h3>完美的管理方式</h3>
<p>最新的管理培训方案，让您的企业赶超同行。</p>
</div>
</div>
</div>
</div>
//CSS 部分
.tab2 {
background: #eee;
padding: 60px 20px;
text-align: center;
}
.tab2 img {
width: 40%;
height: 40%;
}
.tab3 {
padding: 40px 0;
text-align: center;
}
.tab3 img {
width: 65%;
height: 65%;
}
.text h3 {
font-size: 20px;
}
.text p {
font-size: 14px;
}
/* 小屏幕（平板，大于等于 768px） */
@media (min-width: 768px) {
.text h3 {font-size: 22px;
}
.text p {
font-size: 15px;
}
.tab2-text {
float: left;
}
.tab2-img {
float: right;
}
}
/* 中等屏幕（桌面显示器，大于等于 992px） */
@media (min-width: 992px) {
.text h3 {
font-size: 24px;
}
.text p {
font-size: 16px;
}
.tab2-text {
float: left;
}
.tab2-img {
float: right;
}
}
/* 大屏幕（大桌面显示器，大于等于 1200px） */
@media (min-width: 1200px) {
.text h2 {
font-size: 26px;
}
.text p {
font-size: 18px;
}
.tab2-text {
float: left;
}
.tab2-img {
float: right;
}
}//JS 控制垂直居中
$('.text').eq(0).css('margin-top', ($('.auto').eq(0).height() -
$('.text').eq(0).height()) / 2 + 'px');
$(window).resize(function() {
$('.text').eq(0).css('margin-top', ($('.auto').eq(0).height() -
$('.text').eq(0).height()) / 2 + 'px');
});
$('.text').eq(1).css('margin-top', ($('.auto').eq(1).height() -
$('.text').eq(1).height()) / 2 + 'px');
$(window).resize(function() {
$('.text').eq(1).css('margin-top', ($('.auto').eq(1).height() -
$('.text'//谷歌浏览器解析的顺序调整，需要全部加载后执行
$(window).load(function () {
$('.text').eq(0).css('margin-top', ($('.auto').eq(0).height() -
$('.text').eq(0).height()) / 2 + 'px');
});
注：对于 Firefox 浏览器，可以按 Ctrl+Shift+M，调整移动端尺寸。
//子栏目标题
<div class="jumbotron">
<div class="container">
<hgroup>
<h1>资讯</h1>
<h4>企业内训的最新动态、资源等...</h4>
</hgroup>
</div>
</div>
//栏目 CSS
.jumbotron {
margin: 50px 0 0 0;
padding: 60px 0;
background: #ccc url(../img/bg.jpg);
color: #ccc;
}
.jumbotron h1 {
font-size: 26px; //768,30; 992,33; 1200,36;
padding: 0 0 0 20px;
}
.jumbotron h4 {
font-size: 16px; //768,16; 992,17; 1200,18
padding: 0 0 0 20px;}
//资讯内容
<div id="information">
<div class="container">
<div class="row">
<div class="col-md-8 info-left">
<div class="container-fluid" style="padding:0;">
<div class="row info-content">
<div class="col-md-5 col-sm-5 col-xs-5">
<img src="img/info1.jpg"
class="img-responsive" alt="">
</div>
<div class="col-md-7 col-sm-7 col-xs-7">
<h4>广电总局发布 TVOS2.0 华为阿里参与研发</h4>
<p class="hidden-xs">TVOS2.0 是在 TVOS1.0 与华
为 MediaOS 及阿里巴巴 YunOS 融合的基础上，打造的新一代智能电视操作系统。华为主要
承担开发工作，内置的电视购物商城由阿里方面负责。</p>
<p>admin 15 / 10 / 11</p>
</div>
</div>
</div>
</div>
<div class="col-md-4 info-right hidden-xs hidden-sm">
<blockquote>
<h2>热门资讯</h2>
</blockquote>
<div class="container-fluid">
<div class="row">
<div class="col-md-5 col-sm-5 col-xs-5"
style="margin:12px 0;padding:0;">
<img src="img/info3.jpg"
class="img-responsive" alt="">
</div>
<div class="col-md-7 col-sm-7 col-xs-7"
style="padding-right:0">
<h4>标题</h4>
<p>admin 15 / 10 / 11</p>
</div>
</div>
</div>
</div>
</div>
</div>//资讯内容 CSS
#information {
padding: 40px 0;
background: #eee;
}
.info-right {
background-color: #fff;
box-shadow: 2px 2px 3px #ccc;
}
.info-right blockquote {
padding: 0;
margin: 0;
}
.info-right h2 {
font-size: 20px;
padding: 5px;
}
.info-right h4 {
line-height: 1.6;
}
.info-content {
background-color: #fff;
box-shadow: 2px 2px 3px #ccc;
margin: 0 0 20px 0;
}
.info-content img {
margin: 12px 0;
}
.info-content h4 {
font-size: 14px; //768,16; 992,18; 1200,20;
padding: 2px 0 0 0;
}
.info-content p {
line-height: 1.6;
color: #666;
}
//对于.info-content h4，在中屏和大屏需要保持一行。
.info-content h4 {
overflow: hidden;
white-space: nowrap;
text-overflow: ellipsis;
}感谢收看本次教).eq(1).height()) / 2 + 'px');
});
```

## 五．资讯内容

```
//谷歌浏览器解析的顺序调整，需要全部加载后执行
$(window).load(function () {
$('.text').eq(0).css('margin-top', ($('.auto').eq(0).height() -
$('.text').eq(0).height()) / 2 + 'px');
});
注：对于 Firefox 浏览器，可以按 Ctrl+Shift+M，调整移动端尺寸。
//子栏目标题
<div class="jumbotron">
<div class="container">
<hgroup>
<h1>资讯</h1>
<h4>企业内训的最新动态、资源等...</h4>
</hgroup>
</div>
</div>
//栏目 CSS
.jumbotron {
margin: 50px 0 0 0;
padding: 60px 0;
background: #ccc url(../img/bg.jpg);
color: #ccc;
}
.jumbotron h1 {
font-size: 26px; //768,30; 992,33; 1200,36;
padding: 0 0 0 20px;
}
.jumbotron h4 {
font-size: 16px; //768,16; 992,17; 1200,18
padding: 0 0 0 20px;}
//资讯内容
<div id="information">
<div class="container">
<div class="row">
<div class="col-md-8 info-left">
<div class="container-fluid" style="padding:0;">
<div class="row info-content">
<div class="col-md-5 col-sm-5 col-xs-5">
<img src="img/info1.jpg"
class="img-responsive" alt="">
</div>
<div class="col-md-7 col-sm-7 col-xs-7">
<h4>广电总局发布 TVOS2.0 华为阿里参与研发</h4>
<p class="hidden-xs">TVOS2.0 是在 TVOS1.0 与华
为 MediaOS 及阿里巴巴 YunOS 融合的基础上，打造的新一代智能电视操作系统。华为主要
承担开发工作，内置的电视购物商城由阿里方面负责。</p>
<p>admin 15 / 10 / 11</p>
</div>
</div>
</div>
</div>
<div class="col-md-4 info-right hidden-xs hidden-sm">
<blockquote>
<h2>热门资讯</h2>
</blockquote>
<div class="container-fluid">
<div class="row">
<div class="col-md-5 col-sm-5 col-xs-5"
style="margin:12px 0;padding:0;">
<img src="img/info3.jpg"
class="img-responsive" alt="">
</div>
<div class="col-md-7 col-sm-7 col-xs-7"
style="padding-right:0">
<h4>标题</h4>
<p>admin 15 / 10 / 11</p>
</div>
</div>
</div>
</div>
</div>
</div>//资讯内容 CSS
#information {
padding: 40px 0;
background: #eee;
}
.info-right {
background-color: #fff;
box-shadow: 2px 2px 3px #ccc;
}
.info-right blockquote {
padding: 0;
margin: 0;
}
.info-right h2 {
font-size: 20px;
padding: 5px;
}
.info-right h4 {
line-height: 1.6;
}
.info-content {
background-color: #fff;
box-shadow: 2px 2px 3px #ccc;
margin: 0 0 20px 0;
}
.info-content img {
margin: 12px 0;
}
.info-content h4 {
font-size: 14px; //768,16; 992,18; 1200,20;
padding: 2px 0 0 0;
}
.info-content p {
line-height: 1.6;
color: #666;
}
//对于.info-content h4，在中屏和大屏需要保持一行。
.info-content h4 {
overflow: hidden;
white-space: nowrap;
text-overflow: ellipsis;
}
```

##  六．案例内容 

```
//案例内容 1-4 个根据不同显示比例展示
<div class="col-lg-3 col-md-4 col-sm-6 col-xs-12 col">
<div class="thumbnail">
<img src="img/case1.jpg" alt="">
<div class="caption">
<h4>中国移动通信</h4>
<p>参与了本机构的总裁管理培训课程，学员反馈意见良好。</p>
</div>
</div>
</div>
//CSS 部分
#case {
padding: 40px 0;
text-align: center;
background-color: #eee;
}
#case h4 {
color: #666;
}
#case p {
color: #666;
line-height: 1.6;
}
#case .col {
margin: 0 0 20px 0;
}
二．关于栏目
//左右两栏即可
<div class="row"><div class="col-md-3 hidden-sm hidden-xs">
<div class="list-group">
<a class="list-group-item" href="#1">1.机构简介</a>
<a class="list-group-item" href="#2">2.加入我们</a>
<a class="list-group-item" href="#3">3.联系方式</a>
</div>
</div>
<div class="col-md-9 about">
<a name="1"></a>
<h3>机构简介</h3>
<p>瓢城企业培训有限公司是一家专业以智能化弱电工程为主的高科技民营
企业，公司自创立以来一直专业致力于智能化弱电工程；始终坚持发扬"诚信、创新、沟通
"为企业宗旨，以"技术、服务"为立业之本的团体精神，并形成一套完整的设计、安装、调
试、培训、维护一站式服务体系。</p>
<a name="2"></a>
<h3>加入我们</h3>
<p>网络已深刻改变着人们的生活，本地化生活服务市场前景巨大，生活半径
团队坚信本地化生活服务与互联网的结合将会成就一家梦幻的公司， 我们脚踏实地的相信梦
想，我们相信你的加入会让生活半径更可能成为那家梦幻公司！生活半径人有梦想，有魄力，
强执行力，但是要实现这个伟大的梦想，需要更多的有创业精神的你一路前行。公司将提供
有竞争力的薪酬、完善的福利（五险一金）、期权、广阔的上升空间。只要你有能力、有激
情、有梦想，愿意付出，愿意与公司共同成长，请加入我们！</p>
<p>请发送您的简历到：hr@xxx.com，我们会在第一时间联系您！</p>
<a name="3"></a>
<h3>联系方式</h3>
<p>地址：江苏省盐城市亭湖区大庆中路 1234 号</p>
<p>邮编：1234567</p>
<p>电话：010-88888888</p>
<p>传真：010-88666666</p>
</div>
</div>
//CSS 部分
#about {
padding: 40px 15px;
background-color: #eee;
}
#about .about {
background-color: #fff;
box-shadow: 2px 2px 3px #ccc;
padding-bottom: 20px;
}
#about h3 {
margin: 0 0 10px 0;padding: 20px 0;
border-bottom: 1px solid #eee;
font-size: 18px; //768,19; 992,20; 1200 22;
}
#about p {
line-height: 2;
font-size: 13px; //768,14; 992,15; 1200 16;
}
```

