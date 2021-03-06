TOPIC: Data Type

# 数据类型

**数据类型**（或**类型**）是影响其可以存储何种数据的值的特征 - 例如，在JavaScript中，布尔类型`Boolean`仅保存真（`true`）和假（`false`）值，而字符串类型`String`可以容纳文本字符串，数字类型`Number`可以容纳任何数字，依此类推。

值的数据类型也会影响对该值的有效操作。例如，整数可以乘以整数，但不能乘以字符串。

## 静态类型

**静态类型**的语言是指**编译程序**（也叫**编译器**）在**编译时**就知道变量类型的语言（例如*[[Java]]*，*C*或 *C++*）。 在大多数这些语言中，类型必须由程序员明确指出；在其他情况下（例如*OCaml*），类型推断允许程序员不指示其变量类型。

## 动态类型

**动态类型**的语言是指**解释程序**（也叫**解释器**）在**运行时**根据当时的变量值为变量动态分配类型，比如[[JavaScript]]。

## 基本类型 (Primitive)

**基本类型**（基本数值、基本数据类型）是一种既非对象也无方法的数据。

多数情况下，基本类型直接代表了**最底层的语言实现**。

所有基本类型的值都是**不可改变**的。但需要注意的是，基本类型本身和一个赋值为基本类型的变量的区别。变量会被赋予一个新值，而原值不能像数组、对象以及函数那样被改变。

## 类型转换

**类型转换**表示将数据从一种数据类型转换成另一种数据类型。“*隐式转换*”发生在编译器自动分配数据类型时，但是源代码也可能明确要求进行转换（即*强制转换*或*显示转换*）。
例如，在给定指令或语句`5 + 2.0`的情况下，将浮点数`2.0`隐式地转换为整数，但在给定指令或语句`Number("0x11")`的情况下，字符串`"0x11"`被显式转换为整数`17`。

## 类型自动转换或类型隐式转换

**类型自动转换**是值从一种数据类型到另一种（例如，*字符串*到*数字*）的*自动*或*隐式*的转换。

例如：

```javascript
const value1 = '5';
const value2 = 9;
let sum = value1 + value2;

console.log(sum);
```

在上面的示例中，JavaScript将数字中的`9`强制转换为字符串，然后将两个值串联在一起，从而产生了字符串`"59"`。 JavaScript可以在字符串或数字之间选择，并决定使用字符串。

编译器可以将5强制转换为数字并返回`14`的总和，但事实并非如此。要返回此结果，您必须使用`Number()`方法将`5`显式转换为数字：

```javascript
sum = Number(value1) + value2;
```

## 更多

- [Data Type - 维基百科](https://en.wikipedia.org/wiki/Data%20type)
- [Type System - 维基百科](https://en.wikipedia.org/wiki/Type%20system)
- [Primitive Data Type - 维基百科](https://en.wikipedia.org/wiki/Primitive%20data%20type)
