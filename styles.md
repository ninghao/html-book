# 样式

页面会用到一些样式，这些样式可以放在样式表里，后面学习 CSS 的时候，我们再详细了解怎么样为页面添加样式。这里先去创建一个样式表，然后把它链接到页面上使用。页面上用的样式表一般放在文档的 head 部分，链接样式用的是 link：

```html
<link rel="stylesheet" href="样式表的路径">
```

link 的 rel 属性的值设置成了 stylesheet，表示这是一个样式表。href 属性的值是这个样式表的位置。

有时可以把样式直接写在 HTML 文档内部，可以把样式放在一组 `<style>` 标签里面：

```html
<style>
  /* 这里是需要的样式 */
</style>
```

## 位置与顺序

链接的样式表一般会放在 &lt;head&gt; 标签里面，也就是文档的头部。要注意链接的样式表的加载顺序很重要，下面的样式表里的样式更有机会覆盖掉在它上面链接的样式表里的样式。

## 编辑技巧

编辑器上安装了 emmet 插件以后，输入 `link` ，按一下 tab，就可以快速得到链接样式表的 HTML 代码。

## 练习

创建一个样式文件，放在项目下的 styles 目录里面，样式表的名字是 main.css，然后打开 index.html 这个文档，在 head 标签里，链接使用这个样式表：

```html
<head>
  <meta charset="UTF-8">
  <title>Document</title>
  <link rel="stylesheet" href="styles/main.css">
</head>
```

打开 styles/main.css，在这个样式表文件里添加下面样式代码：

```css
body {
  background: #f8f8f8;
}
```

保存样式表文件，在浏览器上预览页面的变化，你会发现页面会用一种浅灰色作为背景。

