设置内联样式与获取类似，都是通过 style 属性或 setAttribute() 方法实现。

## style 属性方式

设置内联样式，依旧是通过 HTML 页面元素的 style 属性实现。

```javascript
element.style = style;

我们可以通过以下示例代码，学习如何通过 style 属性设置内联样式:

```html
<p id="p1" style="color: lightcoral;font-weight: bolder">这是一个段落内容.</p>
```

> **值得注意的是:** 这种方式定义 CSS 样式，是字符串类型。并不适用于定义过多的 CSS 样式属性。

## setAttirbute() 方法方式

通过 style 属性设置内联样式，我们还可以调用 element.setAttribute() 方法实现。
<p id="p1" style="color: lightcoral;font-weight: bolder">这是一个段落内容.</p>
```

> **值得注意的是:** 通过 setAttribute() 方法设置内联样式同样是字符串类型。

## CSSStyleDeclaration 对象

CSSStyleDeclaration 对象提供的属性和方法可以帮助我们设置 CSS 样式的具体内容。
| --- | --- |
| setProperty() | 为指定的 CSS 样式属性设置一个新的值。|
| removeProperty() | 删除指定的 CSS 样式属性。|

### setProperty() 方法

```javascript
style.setProperty(propertyName, value, priority);
```

上述语法结构中，作为参数的 propertyName 表示要修改的 CSS 样式属性名称。

value 是可选的，表示为修改的 CSS 样式属性新的值。如果没有设置任何值，则表示空字符串。

参数 priority 也是可选的，表示设置 CSS 样式的优先级别。

我们可以通过以下示例代码，学习如何通过 setProperty() 方法设置 CSS 的样式属性:

```html
<p id="p1" style="color: lightcoral;font-weight: bolder">这是一个段落内容.</p>
```

### removeProperty() 方法

```javascript
var oldValue = style.removeProperty(property);
```

上述语法结构中，作为参数的 property 表示要删除的 CSS 样式属性名称，作为返回值的 oldValue 表示删除的样式属性的值。

我们可以通过以下示例代码，学习如何通过 removeProperty() 方法删除 CSS 的样式属性:

```html
<p id="p1" style="color: lightcoral;font-weight: bolder">这是一个段落内容.</p>
```