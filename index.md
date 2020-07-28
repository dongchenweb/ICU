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
* { /* 对页面进行初始化 */
	margin: 0;
	padding: 0;
}

.menu{
	background-color:yellow;
	width:100%;
	height:35px;
}
.nav{
	float:left;
	margin-left:15px;
}
ul, a {											/* 菜单栏的具体设计 */
	font-size: 30px;
	list-style: none;
	text-decoration: none;
	background-color: #1F1F1F;
	color: red;
	width: 100px;
	text-align: center;
	border: 0px solid black;
	border-radius: 5px; /* 圆角 */
	margin-top: 0px;
}

a {
	dispaly: block;
}

.submenu{										/* 下拉菜单的隐藏 */
	display:none;
}

.nav:hover .submenu{							/* 使用hover选择器，实现鼠标移至标签上时显示隐藏内容 */
	display:block;
	clear:both;
}

.window{										/* 主窗口的div设计 */
	background-color:#11ffff;
	width:100%;
	padding:50% 0 0;
}
</style>
</head>
<body>
	<div class="menu">
		<ul class="nav">
			<a href="#">一号房</a>
			<ul class="submenu">
				<li><a href="#">周潮</a></li>
				<li><a href="#">炸炸</a></li>
				<li><a href="#">冬晨</a></li>
				<li><a href="#">老军医</a></li>
				<li><a href="#">林学宇</a></li>
			</ul>
		</ul>
		<ul class="nav">
			<a href="#">二号房</a>
			<ul class="submenu">
				<li><a href="#">周潮</a></li>
				<li><a href="#">炸炸</a></li>
				<li><a href="#">冬晨</a></li>
				<li><a href="#">老军医</a></li>
				<li><a href="#">林学宇</a></li>
			</ul>
		</ul>
		<ul class="nav">
			<a href="#">三号房</a>
			<ul class="submenu">
				<li><a href="#">周潮</a></li>
				<li><a href="#">炸炸</a></li>
				<li><a href="#">冬晨</a></li>
				<li><a href="#">老军医</a></li>
				<li><a href="#">林学宇</a></li>
			</ul>
		</ul>
		<ul class="nav">
			<a href="#">四号房</a>
			<ul class="submenu">
				<li><a href="#">周潮</a></li>
				<li><a href="#">炸炸</a></li>
				<li><a href="#">冬晨</a></li>
				<li><a href="#">老军医</a></li>
				<li><a href="#">林学宇</a></li>
			</ul>
		</ul>
		<ul class="nav">
			<a href="#">五号房</a>
			<ul class="submenu">
				<li><a href="#">周潮</a></li>
				<li><a href="#">炸炸</a></li>
				<li><a href="#">冬晨</a></li>
				<li><a href="#">老军医</a></li>
				<li><a href="#">林学宇</a></li>
			</ul>
		</ul>
	</div>
	<div class="window">
	</div>
</body>
</html>
