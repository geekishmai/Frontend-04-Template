
## 运算符优先级—产生树
### Member
	1. a.b
	2. a[b]
	3. foo`string`
	4. new.target
	5. new Foo

### 引用类型 Reference
> 可以理解成  可以XX.XXX的类型

 == Boolean会转换为Number再判断 

 ## 类型转换
 boxing && unboxing

 ## 运行时
 - [[type]]: normal, break, continue, return, or throw
 - [[value]]: 基本类型
 - [[target]]: label

 ## 简单语句/复合语句
 ### 控制语句 （流程）
 - Throw
throw new Error()
 - Continue
 - Break
 - Return

 ### 复合语句
 - if
 - block
 - switch
 - iteration
 for/while
 - label
 - try，catch，finary（不会被return打断）

label搭配break使用，跳出多层循环


### 声明
- function
- function *
- async function
- var 函数级变量、
- let
- const  不能在声明前使用
- class

预处理  声明会被拉到函数的作用集

### 作用域
 - 大函数 
 > 在函数内使用{}把函数切分为小节，


## 结构化设计
### 执行粒度
- 宏任务
- 微任务（Promise）
- 函数调用
- 语句/声明

#### 宏任务微任务
Tasks, microtasks, queues and schedules[https://jakearchibald.com/2015/tasks-microtasks-queues-and-schedules/]
### 函数调用
所有的内置对象都会放进 Realm 在不同的 Realm 实例之间，完全互相独立