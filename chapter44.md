第四十四章 继续玩（一）
===

上一节写的网页我自己也情不自禁的玩了起来，然后自己把自己气坏了，喵的，真的点不着！后来给自己写了一个作弊器才算完事。

今天干点更气人的，要是我自己把自己气坏了，你们要补偿我！！！今天我就是要不畏艰辛，做一只虫子！嗯，就是一只一伸一缩，爬啊爬的虫子。

对了，画虫子怪麻烦的。一节一节的身体，毛茸茸的，还要有好多腿……好恶心……，喵的我偷点懒，做一只简单的虫子，你们别介意哈~

所以我决定，用一个绿色的矩形当虫子好了（好简单地说！）。好，我们来写一条虫子……为什么是写一只虫子……老好看了！

	<!DOCTYPE html>
	<html lang="en">
		<head>
			<meta charset="UTF-8">
			<title>我是一只小虫子，不呀不着急</title>
			<style>
				#cz {
					position: absolute;
					left: 10px;
					top: 50px;
					height: 5px;
					width: 15px;
					background:#393;
				}
			</style>
			<script src="http://upcdn.b0.upaiyun.com/libs/jquery/jquery-2.0.3.min.js"></script>
			<script type = "text/javascript">
				$(document).ready(function(){
					一会在这写代码
				});
			</script>
		</head>
		<body>
			<div id="cz"></div>
		</body>
	</html>

这是一个 15×5 像素的绿色虫子，嗯，我就说他是虫子，有本事你咬我啊？现在我们来研究虫子怎么往前爬啊，这是怎样一个过程呢？首先，虫子把脑袋伸出去（头前进，尾不动），然后虫子脑袋不动，把尾巴缩回来（头不动，尾前进），如此往复，方得前行。然后我们就来做这些事情啊。

第一步，头前进，尾不动。这不就是变长吗？

	$("#cz").animate({width:'20px'},1000);

来解释这个能让你受用终身的句子：animate 动画的意思，他可以对几乎所有的 css 属性进行动画动作，爽歪啊~

后面的大括号里是要改变的 css 属性，就是从现有的值，变到这里给出的值。嗯，动画就是指这个变化的过程。格式有了，大家照着抄就是了啊。需要注意的是啊，如何是 margin-top 这样带有连接线的属性要换个写法啊，变成这样 marginTop 这样。

然后再后面的一个逗号和 1000 是什么意思呢？逗号是分割两个参数，前面说那里发生变化，说完了，逗号分隔一下，然后下一个参数，动画的速度，就是要用多长时间完成这个动画啊。这个时间单位是毫秒，像我这里写的 1000 其实就是一秒啦（1秒 = 1000 毫秒）。

然后呢，这句代码的意思是，#cz 花费一秒的时间，动态的将宽度（width）从原来的值（15px）变到指定的值（20px）。

来试试效果哦，当然这个变化不太明显，要仔细看才能看得到，不过你要是只是想看效果，可以先把上面语句中的 20px 换成 300px，然后是刷新页面看看，就很明显了。

这句我们就学明白了，然后，我们下节课再废话下一个步骤。