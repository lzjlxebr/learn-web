# let和const命令（3）
## let命令
* 只在代码块内有效
* 不存在变量提升
* 暂时性死区，再作用域内，在 `let` 声明变量之前调用会报错，`typeof` 也会报错
* 不允许重复声明

## 块级作用域
* `let` 会创建块级作用域
* 防止变量泄漏

## const命令
* 声明常量，其他规则类似于 `let`
* 用 `const` 命令声明的对象，不可改变所指地址，对象属性可以改变
* es6声明变量的六种方法 `var` `function` `let` `const` `import` `class`

## 环境顶层对象
* 浏览: `window`
* node: `global`
* `var` `function` 声明的对象为全局对象，同时也是顶层对象的属性
* `let` `const` `class` 声明的对象不挂在顶层对象下面，将全局变量与顶层对象的属性脱钩