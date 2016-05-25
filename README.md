### 移动端 - 日期面板选择器
使用说明:
1. 在页面上引入 css 和 js (可以参考index.html)
```
<link rel="stylesheet" type="text/css" href="css/mdate.css">
<script type="text/javascript" src="js/jquery.js"></script>
<script type="text/javascript" src="js/mdate.js"></script>
```

2. 在页面上使用 `input[type="text"]` 作为输入框,此外为了防止手机上弹出软件盘,添加 `readonly` 属性
```
<input id="in" type="text" readonly></input>
```

3. 日期组件初始化
```
$(function() {
	var opts = {
		minDate: new Date(2016,00,01),
		maxDate: new Date(2016,02,09),
	};
	$('#in').mdater(opts);
});
```
