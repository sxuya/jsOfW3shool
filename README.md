# jsOfW3shool
summary and log when learning on w3school.com.cn



## 好处

- 使用外部 script 的好处:
  - 分离 HTML 和 代码
  - 使 HTML 和 JS 更易于阅读和维护
  - 已经缓存的 JS 文件可**加速**网页加载



## 注意点

- JS 不提供任何 **内建** 的打印或者显示函数. 解决方法是:
  - 使用 window.alert() 写入警告框 (**先**显示 alert 内容, **再**其他内容显示)
  - 使用 document.write() 写入 HTML 输出 **(仅仅用于测试)**
  - 使用 innerHTML 写入 HTML 元素
  - 使用 console.log() 写入浏览器控制台
- JS 对大小写敏感, 比如 lastname 和 lastName 是两个不同的变量; 不会把 VAR 翻译成关键词 var
- ``` 数字1 + 数字2 + 字符串 + 数字3 + 数字4```, 数字1 和 数字2 会进行运算, 数字3 和 数字4 不会进行运算, 整体最后都会变成 字符串.
- JS 从 0\~11 表示 一月\~十二月, 所以: 2020,12 就是 2021年1月
- 1 秒 = 1000 毫秒
- 作用域。除非有意为之，否则请勿创建全局变量（或函数，能够覆盖 window 变量或函数；任何函数，包括 window 对象，能够覆盖全局变量和函数。）
- 提升 hoisting
  - var x = 8; // 放在 code 之后，code 只能使用 y、而没有 值8。
  - 参考连接：https://www.w3school.com.cn/js/js_hoisting.asp
  - let / const 没有 提升 hoisting 作用。
- coding conventions
  - 缩进使用 4 个空格, 而不是 tab. 不同的编译器对 tab 的解释也不尽相同.
- 数据类型: 松散类型.
- switch 中使用的是「严格比较 ===」
- return 不可以换行!
- JS 不支持带有命名索引的数组; 对象使用命名索引.
- 函数执行
  - 定义 时候, 内部的代码不会执行;
  - 调用 时候,内部的代码会被执行.
- 



## 习惯

- JS 语句过长, 可以直接拆行, 拆行的最佳位置是某个运算符
- 在脚本的开头声明所有变量是个好习惯.
- coding conventions
  - 勿使用 new Object()
    - {} 代替 new Object()
    - "" 代替 new String()
    - 0 代替 new Number()
    - false 代替 new Boolean()
    - [] 代替 new Array()
    - /()/ 代替 new RegExp()
    - function(){} 代替 new Function()
  - 实例
    - var x1 = {};
    - var x2 = "";
    - var x3 = 0;
    - var x4 = false;
    - var x5 = [];
    - var x6 = /()/;
    - var x7 = function(){};
- 



## 方法

- 浮点偏差
  - 偏差: 0,1 + 0.2 = 0.3000000004
  - 解决方法: 使用乘除运算. (0.1 * 10 + 0.2 * 10) / 10
- 循环性能改善
  - 差的代码: ``` var i; for (i = 0; i < arr.lenght; i++) {}```
  - 更好的代码: ``` var i; var l = arr.lenght; for ( i = 0; i < l; i++) {}```
  - 原因: 包括 for 语句, 每次循环都会执行.

## 暂时不明

- Math 构造器. 与其他全局对象不同，Math对象没有构造函数。方法和属性是静态的。可以在不首先创建Math对象的情况下使用所有方法和属性（常量）。
- 