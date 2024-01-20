# Learn Rust by Building Real Applications

网站：https://www.udemy.com/course/rust-fundamentals/

作者：Lyubomir Gavadinov

https://www.koudaizy.com/tutorials/rust-fundamentals/

Rust is a modern systems programming language.
	Memory safe
	No Null
	No Exceptions
	Modern package manager
	No Data Races

doc.rust-lang.org/book/#the-rust-programming-language

`cargo install cargo-expand`

`cargo expand`

`rustup toolchain list`

`rustup toolchain install nightly-x86_64-unknown=linux=gnu`

`rustup toolchain install stable-aarch64-apple-darwin`

Memory Management
	The Stack 栈
	The Heap 堆
	Pointers 指针
	Smart Pointers 智能指针

What is the stack: It's a special region of the process memory that stores variables created by each function.

What is the heap: It's a region of the process memory that is NOT automatically managed.



----

# Rust权威指南 The Rust Programming Language

## 第 1 章 入门指南

Cargo是Rust工具链中内置的构建系统及包管理器。
### 使用cargo
`cargo new xx_xx`
`cargo run`
`cargo build`
`cargo check`

cargo使用TOML(Tom's Obvious, Minimal Language)作为标准的配置格式。

从Git检出代码、将当前目录移动到该项目的目录下及执行构建操作。
```bash
git clone someurl.com/someproject
cd someproject
cargo build
```

## 第 2 章 编写一个猜数游戏














## 所有权

所有权及其相关功能：借用、切片，以及Rust在内存中布局数据的方式

栈与堆

所有权规则
	Rust中的每一个值都有一个对应的变量作为它的所有者。
	在同一时间内，值有且仅有一个所有者。
	当所有者离开自己的作用域时，它持有的值就会被释放掉。

String类型
字符串字面量是不可变的；并不是所有字符串的值都能在编写代码时确定。

不同于拥有垃圾回收机制的语言，Rust中：内存会自动地在拥有它的变量离开作用域后进行释放。

Rust会在作用域结束的地方自动调用drop函数。

Rust永远不会自动创建数据的深度拷贝。
移动(move)
克隆(clone)

Copy trait
Drop trait

所有权与函数：将值传递给函数在语义上类似于对变量进行赋值。

将一个值赋值给另一个变量时就会转移所有权。
可以利用元组来返回多个值

引用和借用



















