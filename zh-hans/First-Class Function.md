TOPIC: First-Class Function
AUTHORS: Yuns Xie; yuns.xie@qq.com; github:theprimone
         蒋璇; 645762213@qq.com; github:Jiang-Xuan
         itplus; eforegist@github.com; github:eforegist

# 头等函数

当一门编程语言的函数可以被当作变量一样用时，则称这门语言拥有头等函数。例如，在这门语言中，函数可以被当作参数传递给其他函数，可以作为另一个函数的返回值，还可以被赋值给一个变量。

## 示例 | 把函数赋值给变量

JavaScript

```javascript
const foo = function() {
   console.log("foobar");
}
// 用变量来调用它
foo();
```

这里我们把一个匿名函数赋值给一个变量，然后我们在这个变量后面加上一对圆括号 `()` 来调用这个函数。

!!! note
    即使你的函数有自己的函数名称，你仍然可以用这个变量名去调用它。给函数命名只会方便你调试，但不会影响我们调用它。

## 示例 | 传递一个函数作为参数

JavaScript

```javascript
function sayHello() {
   return "Hello, ";
}
function greeting(helloMessage, name) {
  console.log(helloMessage() + name);
}
// 传递 `sayHello` 作为 `greeting` 函数的参数
greeting(sayHello, "JavaScript!");
```

这里我们传递 `sayHello()` 函数作为 `greeting()` 函数的参数，这就印证了头等函数定义所说的——我们把函数当作 值 或者说是 变量 来对待。

!!! note
    回调函数：我们把一个函数作为参数传递给另外一个函数，那么我们就称这个函数为回调函数。`sayHello()` 函数就是一个回调函数。

## 示例 | 返回一个函数

JavaScript

```javascript
function sayHello() {
   return function() {
      console.log("Hello!");
   }
}
```

在这个例子中，我们需要从另外一个函数中返回一个函数，我们可以返回一个函数，因为在 Javascript 中我们以一个 值 来对待函数。

!!! note
    高阶函数(**Higher-Order Function**)：一个函数返回另外一个函数我们称它为高阶函数。

我们再来看看上面的例子：假如我们需要调用 `sayHello` 这个函数，然后让它返回一个 匿名函数，我们有两种方法：

1- 用一个变量

```javascript
const sayHello = function() {
   return function() {
      console.log("Hello!");
   }
}
const myFunc = sayHello();
myFunc();
```

用这种方法，它返回一个 `Hello!` 的消息。

!!! note
    你要用另外一个变量来调用它。如果你直接用 `sayHello` 来调用这个函数，它会返回这个函数自身，而不会调用它里面被返回的函数。

2- 使用双括号

```javascript
function sayHello() {
   return function() {
      console.log("Hello!");
   }
}
sayHello()();
```

我们使用双括号 `()()` 来调用它里面被返回的函数。