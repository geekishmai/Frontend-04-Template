学习笔记
	◦	1. 做过赋值的话，尽量使用Null（赋空值），undefined不要用于赋值
	◦	2. symbol代替String，用于Object属性名的特别类型
	◦	3. typeof（null）  返回Object
	◦	4. Number类型 — IEEE 754
	⁃	sign（1）
	⁃	Exponent（11）指数位，11111 11111
	⁃	Fraction 实际

	⁃	精度损失

0.1 + 0.2 不等于 0.3 是3次转换，还有一次运算造成的


0.toString()  补充为 0.0toSting

	◦	String
	⁃	character
	⁃	ASCII  127个基础字符
	⁃	Unicode编码   分片区分配语言   UTF-8
	⁃	GB2312  与 Unicode不兼容
	⁃	“”内可以放‘’（可以互换）

	◦	Object对象
	⁃	在设计对象的状态和行为时，遵循“行为改变状态”原则
	⁃	原型机制：如果对象不包含该属性，则会到原型中去链式寻找直到null


	⁃	面向对象的方式


	⁃	创建对象（Function），会有call行为

	•	固有对象（Intrinsic Objects ）：由标准规定，随着 JavaScript 运行时创建而自动创建的对象实例。
	•	宿主对象（host Objects）：由 JavaScript 宿主环境提供的对象，它们的行为完全由宿主环境决定。
	•	内置对象（Built-in Objects）：由 JavaScript 语言提供的对象。
	•	原生对象（Native Objects）：可以由用户通过 Array、RegExp 等内置构造器或者特殊语法创建的对象。
	•	普通对象（Ordinary Objects）：由{}语法、Object 构造器或者 class 关键字定义类创建的对象，它能够被原型继承。

Array：Array 的 length 属性根据最大的下标自动发生变化。
Object.prototype：作为所有正常对象的默认原型，不能再给它设置原型了。
String：为了支持下标运算，String 的正整数属性访问会去字符串里查找。
Arguments：arguments 的非负整数型下标属性跟对应的变量联动。
模块的 namespace 对象：特殊的地方非常多，跟一般对象完全不一样，尽量只用于 import 吧。
类型数组和数组缓冲区：跟内存块相关联，下标运算比较特殊。
bind 后的 function：跟原来的函数相关联。