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



## 习惯

- JS 语句过长, 可以直接拆行, 拆行的最佳位置是某个运算符
- 在脚本的开头声明所有变量是个好习惯.
- 



## 暂时不明

- Math 构造器. 与其他全局对象不同，Math对象没有构造函数。方法和属性是静态的。可以在不首先创建Math对象的情况下使用所有方法和属性（常量）。
- 