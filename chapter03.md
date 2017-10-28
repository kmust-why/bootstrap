## 一．表格

Bootstrap 提供了一些丰富的表格样式供开发者使用。

1. 基本格式

```
//实现基本的表格样式
<table class="table">
```

注：我们可以通过 Firebug 查看相应的 CSS。

2. 条纹状表格

```
//让<tbody>里的行产生一行隔一行加单色背景效果
<table class="table table-striped">
```

注：表格效果需要基于基本格式.table

3. 带边框的表格

```
//给表格增加边框
<table class="table table-bordered">
```

4. 悬停鼠标

```
//让<tbody>下的表格悬停鼠标实现背景效果
<table class="table table-hover">
```

5. 状态类

```
//可以单独设置每一行的背景样式
<tr class="success">
```

注：一共五种不同的样式可供选择。 

|   样式    |        说明         |
| :-----: | :---------------: |
| active  |    鼠标悬停在行或单元格上    |
| success |    标识成功或积极的动作     |
|  info   |   标识普通的提示信息或动作    |
| warning |    标识警告或需要用户注意    |
| danger  | 表示危险或潜在的带来负面影响的动作 |

6. 隐藏某一行

```
//隐藏行
<tr class="sr-only">
```

7. 响应式表格

```
//表格父元素设置响应式，小于 768px 出现边框
<body class="table-responsive">
```

## 二．按钮

Bootstrap 提供了很多丰富按钮供开发者使用。

1. 可作为按钮使用的标签或元素

```
//转化成普通按钮
<a href="###" class="btn btn-default">Link</a>
<button class="btn btn-default">Button</button>
<input type="button" class="btn btn-default" value="input">
```

注意事项有三点：
- 针对组件的注意事项
  虽然按钮类可以应用到a和button元素上，但是，导航和导航条组件只支持
  button元素。

- 链接被作为按钮使用时的注意事项
  如果 a元素被作为按钮使用 ，并用于在当前页面触发某些功能 ，而不是用于
  链接其他页面或链接当前页面中的其他部分，那么，务必为其设置 role="button" 属性。

- 跨浏览器展现

  总结的最佳实践是：**强烈建议尽可能使用 button元素**来获得在各个浏览器上
  获得相匹配的绘制效果。

另外，发现了 Firefox <30 版本的浏览器上出现的一个 bug，其表现是：阻止我们为基于 input 元素所创建的按钮设置 line-height 属性，这就导致在Firefox 浏览器上不能完全和其他按钮保持一致的高度。

2. 预定义样式

```
 //一般信息
 <button class="btn btn-info">Button</button> 
```

|     样式      |   说明   |
| :---------: | :----: |
| btn-default |  默认样式  |
| btn-success |  成功样式  |
|  btn-info   | 一般信息样式 |
| btn-waring  |  警告样式  |
| btn-danger  |  危险样式  |
| btn-primary | 首选项样式  |
|  btn-link   |  链接样式  |

3. 尺寸大小

```
//从大到小的尺寸
<button class="btn btn-lg">Button</button>
<button class="btn">Button</button>
<button class="btn btn-sm">Button</button>
<button class="btn btn-xs">Button</button>
```

4. 块级按钮

```
//块级换行
<button class="btn btn-block">Button</button>
<button class="btn btn-block">Button</button>
```

5. 激活状态

```
//激活按钮
<button class="btn active">Button</button>
```

6. 禁用状态

```
//禁用按钮
<button class="btn active disabled">Button</button> 
```

