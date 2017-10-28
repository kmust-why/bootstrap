## 一．弹出框

弹出框即点击一个元素弹出一个包含标题和内容的容器。 

```
//基本用法
<button class="btn btn-lg btn-danger"
type="button"
data-toggle="popover"
title="弹出框"
data-content="这是一个弹出框插件">
点击弹出/隐藏弹出框
</button>
//JavaScript 初始化
$('button').popover();
```

弹出框插件有很多属性来配置提示的显示，具体如下：

| 属性名                 | 描述                                       |
| ------------------- | ---------------------------------------- |
| data-animation      | 默认 true，在 popover 上应用一个 CSS fade 动画。如果设置 false，则不应用。 |
| data-html           | 默认 false，不允许提示内容格式为 html。如果设置为 true，则可以设置 html 格式的提示内容。 |
| data-placement      | 默认值 top，还有 bottom、left、right 和 auto。如果 auto 会自行调整合适的位置， 如果是 auto left则会尽量在左边显示，但左边不行就靠右边。 |
| data-selector       | 默认 false，可以选择绑定指定的选择器。                   |
| data-original-title | 默认空字符串，弹出框的标题。优先级比 title 低               |
| title               | 默认字空符串，弹出框的标题。                           |
| data-trigger        | 默认值 click，表示怎么触发 popover，其他值为：hover、focus、manual。多个值用空格隔开，manual手动不能和其他同时设置。 |

| data-delay     | 默认值 0，延迟触发 popover(毫秒)，如果传数字则，表示 show/hide 的毫秒数，如果传对象，结构为：{show:500,hide:100} |
| -------------- | ---------------------------------------- |
| data-container | 默认值 false，将 popover 附加到特定的元素上。比如组合按钮组提示，容器不够，可以附加 body 上。container : 'body' |
| data-template  | 更改提示框的 HTML 提示语的模版，默认值为：<divclass="popover"><divclass="arrow"></div><h3class="popover-title"></h3><divclass="popover-content"></div></div> |
| data-content   | 默认值为空，弹出框的内容。                            |
| data-viewport  | 设置外围容器的边际，具体代码看示例。                       |

```
$('button').popover({
container : 'body',
viewport : {
selector : '#view',
padding : 10,
}
});
通过 JavaScript 执行的方法有四个。
//显示
$('button').popover('show');
//隐藏
$('button').popover('hide');
//反转显示和隐藏
$('button').popover('toggle');
//隐藏并销毁
$('button').popover('destroy');
```

Popover 插件中事件有两种。

| 事件类型              | 描述             |
| ----------------- | -------------- |
| show.bs.popover   | 在调用 show 方法时触发 |
| shown.bs.popover  | 在显示整个弹窗时时触发    |
| hide.bs.popover   | 在调用 hide 方法时触发 |
| hidden.bs.popover | 在完全关闭整个弹出时触发   |

```
//事件，其他雷同
$('button').on('show.bs.tab', function () {
alert('调用 show 方法时触发！');
});
```

## 二．警告框

警告框即为点击小时的信息框。 

```
//基本实例
<div class="alert alert-warning">
<button class="close" type="button" data-dismiss="alert">
<span>&times;</span>
</button>
<p>警告：您的浏览器不支持！</p>
</div>
//添加淡入淡出效果
<div class="alert alert-warning fade in">
如果用 JavaScript，可以代替 data-dismiss="alert"
//JavaScript 方法
$('.close').on('click', function () {
$('#alert').alert('close');
})
```

Alert 插件中事件有四种。

| 事件类型            | 描述                 |
| --------------- | ------------------ |
| close.bs.alert  | 当 close 方法被调用后立即触发 |
| closed.bs.alert | 当警告框被完全关闭后立即触发     |

```
//事件，其他雷同
$('#alert').on('close.bs.alert', function () {
alert('当 close 方法被触发时调用！');
});
```

