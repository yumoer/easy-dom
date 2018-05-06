## 回顾什么是外联样式

所谓外联样式，就是在 HTML 页面中内嵌样式表或者引入外部样式文件，再通过 CSS 选择器定位 HTML 页面元素，为其定义样式。

```html
<link rel="stylesheet" href="css/style.css">
```

上述示例代码，通过 `<link>` 元素引入外部的样式表。

```html
<style>
```

上述示例代码，通过 `<style>` 元素定义内嵌样式表。

## Document 对象的 styleSheets 属性

```javascript
var styleSheetList = document.styleSheets;
```

上述语法结构中，作为返回值的 styleSheetList 是一个由 styleSheet 对象组成的列表，每个 styleSheet 对象表示 HTML 页面中内嵌样式表或外联样式表。

```javascript
console.log(document.styleSheets);
```

上述示例代码输出的结果如下:

![](images/06.png)

## StyleSheetList 对象

```javascript
var styleSheetList = document.styleSheets;
```

上述示例代码中，每次循环得到的是 StyleSheet 对象。

## CSSStyleSheet 对象

```javascript
console.log(document.styleSheets[0]);
```

上述示例代码输出的结果如下:

![](images/07.png)

## CSSRuleList 对象

```javascript
var styleSheet = document.styleSheets[0];
```

上述示例代码中，每次循环得到是 CSSRule 对象。

## CSSRule 对象

```javascript
console.log(document.styleSheets[1].cssRules[0]);
```

上述示例代码输出的结果如下:

![](images/08.png)

