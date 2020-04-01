# CSS

## 选择器

- id选择器
    - CSS 中 id 选择器以 "#" 来定义, 即 #{id} 或 tag#{id}
- class选择器，类选择器以一个点"."号显示
    - .{class} 或 tag.{class}

## css 创建
### 外部样式表(external style sheet)
```
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>

浏览器会从文件 mystyle.css 中读到样式声明，并根据它来格式文档。

外部样式表可以在任何文本编辑器中进行编辑。文件不能包含任何的 html 标签。样式表应该以 .css 扩展名进行保存。
```

### 内部样式表(internal style sheet)
```
当单个文档需要特殊的样式时，就应该使用内部样式表。你可以使用 <style> 标签在文档头部定义内部样式表:

<head>
<style>
hr {color:sienna;}
p {margin-left:20px;}
body {background-image:url("images/back40.gif");}
</style>
</head>

```

### 内联样式(inline style)
```
由于要将表现和内容混杂在一起，内联样式会损失掉样式表的许多优势。请慎用这种方法，例如当样式仅需要在一个元素上应用一次时。

要使用内联样式，你需要在相关的标签内使用样式（style）属性。Style 属性可以包含任何 CSS 属性。本例展示如何改变段落的颜色和左外边距：

<p style="color:sienna;margin-left:20px">这是一个段落。</p>
```

### 多重样式优先级
```
(内联样式）Inline style > （内部样式）Internal style sheet >（外部样式）External style sheet > 浏览器默认样式
```