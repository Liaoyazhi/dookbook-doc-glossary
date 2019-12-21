TOPIC: JavaScript

# JavaScript编程语言

JavaScript (JS) 是一种编程语言，为通常用于客户端（client-side）的网页动态脚本，不过，也常通过像[Node.js](http://nodejs.org/)这样的包，用于服务器端（server-side）。

不应该把JavaScript和[[Java]]混淆。“Java”和“JavaScript”都是Oracle（甲骨文）公司在美国和其他国家注册的商标，但是这两种编程语言在语法、语义和使用方面都明显不同。

## 历史

*Brendan Eich*（彼时受雇于Netscape（网景）公司）为服务器端构想的语言JavaScript，不久却在1995年9月加入*Netscape Navigator 2.0*项目。
JavaScript很快获得了成功，而Internet Explorer 3.0也在1996年8月引入了对JavaScript的支持，冠以*JScript*之名。

1996年11月，Netscape开始与[[ECMA]]国际化组织合作以使JavaScript成为行业标准。从此以后，标准化的JavaScript就被称为 *[[ECMAScript]]*，并规范于
**ECMA-262**之下。

## 应用场景

JavaScript通常用于*浏览器*，使开发者能通过[[DOM]]来操纵网页内容、或透过[[AJAX与IndexedDB来操作数据；还可以用它在canvas上面绘图、通过各种APIs与运行浏览器的
各种设备交互等等。由于近年来的发展、以及各浏览器的APIs性能改善，JavaScript成了世界上最常用的编程语言之一。

最近，JavaScript的流行程度 ，由于 **[Node.js](http://nodejs.org/)**平台 —— 这个除浏览器外最流行的跨平台JavaScript运行环境 —— 的成功而大大提升。
Node.js使开发者可以在PC上使用JavaScript作为脚本语言使用以自动化处理和构建功能完备的[[HTTP]]和[[WebSocket]]服务器。

## 面向对象

JavaScript是高度**面向对象**的。它遵循基于 **`prototype`**的模型（与基于类的模型相反）。

## 动态类型

JavaScript是一种*弱类型*或者说 *[动态语言](/zh-hans/glossary/dynamic_programming_language)*。这意味着你不用提前声明变量的类型，在程序运行过程中，类型会被自动确定。这也意味着你可以使用同一个变量保存不同类型的数据：

```javascript
let foo = 42;    // foo现在是数字
foo     = 'bar'; // foo现在是字符串
foo     = true;  // foo现在是布尔类型
```

## 数据类型

最新的[[ECMAScript]]标准定义了8种数据类型:

- 7种原始类型:
    - [`boolean`](/zh-hans/webfrontend/Boolean)
    - [`null`](/zh-hans/webfrontend/null)
    - [`undefined`](/zh-hans/webfrontend/undefined)
    - `number`
    - `bigint`
    - `string`
    - `symbol` (ECMAScript 2016新增)
- 和`Object`。

### JavaScript中的基本类型的包装对象

除了[`null`](/zh-hans/webfrontend/null)和[`undefined`](/zh-hans/webfrontend/undefined)之外，所有基本类型都有其对应的包装对象：

- `String`为字符串基本类型`string`。
- `Number`为数值基本类型`number`。
- `BigInt`为`bigint`基本类型。
- [`boolean`](/zh-hans/webfrontend/Boolean)为布尔基本类型`boolean`。
- `Symbol`为字面量基本类型。

这个包裹对象的`valueOf()`方法返回基本类型值。

## 了解更多

- [JavaScript - 维基百科](https://en.wikipedia.org/wiki/JavaScript)
- [ECMAScript (ECMA-262)标准](http://www.ecma-international.org/publications/standards/Ecma-262.htm)