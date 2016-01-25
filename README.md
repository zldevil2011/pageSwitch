这是一个网页全屏滚动的插件
也是目前比较流行的网页展示方式

样式设计：
h1,body,html{padding: 0;margin: 0;}

html,body{height: 100%;overflow: hidden;}

container的height: 100%;position: relative;

.section{height: 100%;position: relative;}


首先定义一个容器,div #container

然后定义每一页的内容 div #section页码 div .section

初始化一个section为active

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
