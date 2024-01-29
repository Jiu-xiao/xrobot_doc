---
title: bsp
layout: default
parent: API
nav_order: 1
has_children: true
---

# BSP层接口规范

## 语言

* 所有代码尽量使用C语言编写，但是允许使用C++。

## 返回值

* 运行结果使用bsp_status_t返回，尽量返回准确的错误原因。

## 数据类型

* 表示数据长度时使用size_t而非uint32_t
* 变量无需写入时需要用const修饰
