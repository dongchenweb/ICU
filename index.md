<%@ page language="java" import="java.util.*" pageEncoding="UTF-8"%>
<%
	String path = request.getContextPath();
	String basePath = request.getScheme() + "://" + request.getServerName() + ":" + request.getServerPort()
			+ path + "/";
%>

<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>ICU-VIP皇家病房</title>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<style>
html {
	height: 100%;
}

body {
	height: 100%;
	width: 100%;
}

* {
	margin: 0;
	padding: 0;
}

.top-container { /* 总容器 */ /* 导航栏分为两个模块，登录功能以及其他， */
	background-color: blue; /* 实现方法是在一个大的div下内涵两个div，再在其下 */
	height: 30px; /* 分别设计UL */
	min-width: 100%;
	font-family: 'Tahoma', 'simsun' !important;
	color: red;
	margin: 0;
	z-index: 2; /* z-index:用以z轴的位置0，类似于图层 */
}

.top-wrapper { /* 菜单容器 */
	width: 100%;
	height: 30px;
	margin: auto;
}

.top-left-nav, .user-nav {
	display: inline-block;
	height: 30px;
}

.nav {
	display: inline-block;
	margin: 0 auto;
	padding: 0;
	position: relative;
}

.nav:after {
	content: "";
	display: block;
	clear: both;
	visibility: hidden;
	width: 0px;
	height: 0px;
}

.nav ul, .nav li {
	display: block;
	position: relative;
	margin: 0px;
	padding: 0px;
}

.nav a {
	text-decoration: none;
	display: block;
	text-align: center;
	margin: 0 auto;
}

.first-nav {
	float: left;
	text-align: center;
	display: block;
	margin: 0;
	width: 100px;
}

.sec-nav {
	position: relative;
	display: block;
	text-align: center;
}

.top-left-nav .first-nav { /* 显示具体布局 */
	width: 100px;
	line-height: 30px;
}

.top-left-nav .sec-nav {
	margin: 0px;
	display: none;
	padding: 5px 5px;
	width: 100px;
}

.top-left-nav .first-nav:hover .sec-nav { /* a:hover;鼠标移动到链接上 */
	display: block;
}

.window {
	width: 100%;
	height: 100%;
	box-sizing: boder-box;
	position: relative;
	padding: 47% 0 0;
	background-color: #4FFFFF;
}
</style>
</head>
<body style="margin:0;">
	<!--导航栏一般需要一个容器，设置width:100%适应浏览器的大小变化-->
	<div class="top-container container">
		<!--导航栏wrapper一般设置一个固定大小这样子可以通过margin:auto;实现导航栏水平居中
由于顶层容器是适应浏览器变化宽度，所以可以保持水平导航栏自适应浏览器窗口宽度保持居中-->
		<div class="top-wrapper wrapper">
			<!--这个是普通导航栏的容器，就是除了"立即登陆"和"注册新账号"-->
			<div class="nav top-left-nav">
				<!--开始实现列表-->
				<ul>
					<li class="dropdown first-nav"><span>一号房<i class="icon icon-arrow"></i></span>
						<ul class="sec-nav">
							<li><a href="#">周潮</a></li>
							<!-- ul中的dropdown属性与其下li的href="#"实现下拉菜单的显示 -->
							<li><a href="#">炸炸</a></li>
							<li><a href="#">冬晨</a></li>
							<li><a href="#">老军医</a></li>
							<li><a href="#">林学宇</a></li>
						</ul>
					</li>
					<li class="dropdown first-nav"><span>二号房<i class="icon icon-arrow"></i></span>
						<ul class="sec-nav">
							<li><a href="#">周潮</a></li>
							<li><a href="#">炸炸</a></li>
							<li><a href="#">冬晨</a></li>
							<li><a href="#">老军医</a></li>
							<li><a href="#">林学宇</a></li>
						</ul>
					</li>
					<li class="dropdown first-nav"><span>三号房<i class="icon icon-arrow"></i></span>
						<ul class="sec-nav">
							<li><a href="#">周潮</a></li>
							<li><a href="#">炸炸</a></li>
							<li><a href="#">冬晨</a></li>
							<li><a href="#">老军医</a></li>
							<li><a href="#">林学宇</a></li>
						</ul>
					</li>
					<li class="dropdown first-nav"><span>脑瘫素材<i	class="icon icon-arrow"></i></span>
						<ul class="sec-nav">
							<li><a href="#">I have a 紫苑</a></li>
							<li><a href="#">I have a BKB</a></li>
							<li><a href="#">oh~~~~</a></li>
							<li><a href="#">echo sabre</a></li>
							<li><a href="#">I have a MKB</a></li>
							<li><a href="#">I have a BKB</a></li>
							<li><a href="#">oh~~~~</a></li>
							<li><a href="#">whirlpoor</a></li>
						</ul>
					</li>
					<li class="dropdown first-nav"><span>GHSGHS<i	class="icon icon-arrow"></i></span>
						<ul class="sec-nav">
							<li><a href="#">动图</a></li>
							<li><a href="#">图片</a></li>
							<li><a href="#">视频</a></li>
						</ul>
					</li>
			<div class="nav user-nav">
				<ul>
					<li class="first-nav"><a href="#">立即登录</a></li>
					<li class="first-nav"><a href="#">立即注册</a></li>
				</ul>
			</div>
		</div>
	</div>
	<div class="window">
		
	</div>
</body>
</html>
