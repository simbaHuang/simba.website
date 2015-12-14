# jquery.namespace.webSite

集合了一些网站开发中常见的组件(基于jq)

1、截取字符串
-	
js调用
```js
	$("xxx").limit(num)  //num保留的字符串个数
```
html
```html
	<p e-fun="limit" e-num="10">这里只能显示10个字符，嗯呢呢呢</p>   
```
2、Tab菜单切换
-	
js调用
```js
	$("xxx").tab(options) 
	options = {
		num  : 0,       //默认显示  
        ent  : "click", //默认响应事件  
        choo : "choo",  //选中的类名 
	} 
```
html
```html
	<div e-fun="tab" e-event="click" e-index="0" class="tab">
		<div class="clear">
			<a e-tab-for="nav0">a</a>
			<a e-tab-for="nav1">b</a>
			<a e-tab-for="nav2">c</a>
		</div>
		<div>
			<p e-tab-nav="nav0">a</p>
			<p e-tab-nav="nav1">b</p>
			<p e-tab-nav="nav2">c</p>
		</div>
	</div>  
```
3、div模拟下拉
-	
js调用
```js
	$("xxx").dropBox(options) 
	options = {
		tapType: "click", //默认的点击方式---click,touchend
		    n  : 0,       //默认value初始值  
		ntype  : "name",  //提交的input值得value值    
		speed  : 200,     //下拉框下拉或收起的速度
	} 
```
html
```html
	<div e-fun="dropBox" e-val=0  class="dropBox clear">
		<input class="fms" readonly type="text" />
		<i class="fa fa-chevron-down"></i>
		<ul class="">
			<li>选项1</li>
			<li>选项2</li>
			<li>选项3</li>
		</ul>
	</div>  
```
4、图片式多选框
-	
js调用
```js
	$("xxx").check(options) 
	options = {
		tapType    :  "click",     				  //默认的点击方式---click,touchend
		checkSrc   :  "./images/e-check.png",     //显示的默认图片
		checkedSrc :  "./images/e-checked.png",	  //选中后显示的图片
	} 
```
html
```html
	<div class="" e-fun="check">
		<ul class="checkList">
			<li class="fristCheck"><i e-check-all e-check=0><img src="./images/e-check.png" alt="" />全选</i></li>
			<li class="secCheck clear">
				<i e-check-one e-check=0><img src="./images/e-check.png" alt="" />多选1</i>
				<i e-check-one e-check=0><img src="./images/e-check.png" alt="" />多选2</i>
				<i e-check-one e-check=0><img src="./images/e-check.png" alt="" />多选3</i>
				<i e-check-one e-check=0><img src="./images/e-check.png" alt="" />多选4</i>
			</li>
		</ul>
	</div>  
```

5、后续的自己看吧。。。。不愿写了
