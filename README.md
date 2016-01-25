这是一个网页全屏滚动的插件
也是目前比较流行的网页展示方式

首先定义一个容器,div #container

然后定义每一页的内容 div #section页码 div .section

初始化一个section为active

h1,body,html{padding: 0;margin: 0;}

html,body{height: 100%;overflow: hidden;}



<div id="container">

    <div class="section" id="section0">		
	
    </div>
	
    <div class="section" id="section1">	
	
	</div>
	
	<div class="section" id="section2">
	
	</div>
	
	<div class="section" id="section3">
	
	</div>
	
	<div class="section active" id="section4">
	
	</div>
	
</div>

配置参数：
var defaults = {

		'container' : '#container',//容器
		
		'sections' : '.section',//子容器
		
		'easing' : 'ease',//特效方式，ease-in,ease-out,linear
		
		'duration' : 1000,//每次动画执行的时间
		
		'pagination' : true,//是否显示分页
		
		'loop' : false,//是否循环
		
		'keyboard' : true,//是否支持键盘
		
		'direction' : 'vertical',//滑动的方向 horizontal,vertical,
		
		'onpageSwitch' : function(pagenum){}
		
	};
