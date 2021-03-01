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
- JS 从 0/~11 表示 一月\~十二月, 所以: 2020,12 就是 2021年1月



## 习惯

- JS 语句过长, 可以直接拆行, 拆行的最佳位置是某个运算符
- 在脚本的开头声明所有变量是个好习惯.
- 
