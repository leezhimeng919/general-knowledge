- [JS高程](#JS%E9%AB%98%E7%A8%8B)
  - [1.JavaScript简介](#1JavaScript%E7%AE%80%E4%BB%8B)
    - [JavaScript简史](#JavaScript%E7%AE%80%E5%8F%B2)
    - [JavaScript实现](#JavaScript%E5%AE%9E%E7%8E%B0)
    - [JavaScript版本](#JavaScript%E7%89%88%E6%9C%AC)
  - [2.在HTML中使用JavaScript](#2%E5%9C%A8HTML%E4%B8%AD%E4%BD%BF%E7%94%A8JavaScript)
    - [script元素](#script%E5%85%83%E7%B4%A0)
    - [嵌入代码与外部文件](#%E5%B5%8C%E5%85%A5%E4%BB%A3%E7%A0%81%E4%B8%8E%E5%A4%96%E9%83%A8%E6%96%87%E4%BB%B6)
    - [文档模式](#%E6%96%87%E6%A1%A3%E6%A8%A1%E5%BC%8F)
    - [noscript元素](#noscript%E5%85%83%E7%B4%A0)
  - [3.基础概念](#3%E5%9F%BA%E7%A1%80%E6%A6%82%E5%BF%B5)
    - [语法](#%E8%AF%AD%E6%B3%95)
    - [关键字和保留字](#%E5%85%B3%E9%94%AE%E5%AD%97%E5%92%8C%E4%BF%9D%E7%95%99%E5%AD%97)
    - [变量](#%E5%8F%98%E9%87%8F)
    - [数据类型](#%E6%95%B0%E6%8D%AE%E7%B1%BB%E5%9E%8B)
    - [操作符](#%E6%93%8D%E4%BD%9C%E7%AC%A6)
    - [语句](#%E8%AF%AD%E5%8F%A5)
    - [函数](#%E5%87%BD%E6%95%B0)
  - [4.变量、作用域和内存问题](#4%E5%8F%98%E9%87%8F%E4%BD%9C%E7%94%A8%E5%9F%9F%E5%92%8C%E5%86%85%E5%AD%98%E9%97%AE%E9%A2%98)
    - [基本类型和引用类型的值](#%E5%9F%BA%E6%9C%AC%E7%B1%BB%E5%9E%8B%E5%92%8C%E5%BC%95%E7%94%A8%E7%B1%BB%E5%9E%8B%E7%9A%84%E5%80%BC)
    - [执行环境及作用域](#%E6%89%A7%E8%A1%8C%E7%8E%AF%E5%A2%83%E5%8F%8A%E4%BD%9C%E7%94%A8%E5%9F%9F)
    - [垃圾收集](#%E5%9E%83%E5%9C%BE%E6%94%B6%E9%9B%86)
  - [5.引用类型](#5%E5%BC%95%E7%94%A8%E7%B1%BB%E5%9E%8B)
    - [Object类型](#Object%E7%B1%BB%E5%9E%8B)
    - [Array类型](#Array%E7%B1%BB%E5%9E%8B)
    - [Date类型](#Date%E7%B1%BB%E5%9E%8B)
    - [RegExp类型](#RegExp%E7%B1%BB%E5%9E%8B)
    - [Function类型](#Function%E7%B1%BB%E5%9E%8B)
    - [基本包装类型](#%E5%9F%BA%E6%9C%AC%E5%8C%85%E8%A3%85%E7%B1%BB%E5%9E%8B)
    - [单体内置对象](#%E5%8D%95%E4%BD%93%E5%86%85%E7%BD%AE%E5%AF%B9%E8%B1%A1)
  - [6.面向对象的程序设计](#6%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%9A%84%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1)
    - [理解对象](#%E7%90%86%E8%A7%A3%E5%AF%B9%E8%B1%A1)
    - [创建对象](#%E5%88%9B%E5%BB%BA%E5%AF%B9%E8%B1%A1)
    - [继承](#%E7%BB%A7%E6%89%BF)
  - [7.函数表达式](#7%E5%87%BD%E6%95%B0%E8%A1%A8%E8%BE%BE%E5%BC%8F)
    - [递归](#%E9%80%92%E5%BD%92)
    - [闭包](#%E9%97%AD%E5%8C%85)
    - [模仿块级作用域](#%E6%A8%A1%E4%BB%BF%E5%9D%97%E7%BA%A7%E4%BD%9C%E7%94%A8%E5%9F%9F)
    - [私有变量](#%E7%A7%81%E6%9C%89%E5%8F%98%E9%87%8F)
  - [8.BOM](#8BOM)
    - [Window对象](#Window%E5%AF%B9%E8%B1%A1)
    - [location对象](#location%E5%AF%B9%E8%B1%A1)
    - [navigator对象](#navigator%E5%AF%B9%E8%B1%A1)
    - [screen对象](#screen%E5%AF%B9%E8%B1%A1)
    - [history对象](#history%E5%AF%B9%E8%B1%A1)
  - [9.客户端检测(检测是啥浏览器)](#9%E5%AE%A2%E6%88%B7%E7%AB%AF%E6%A3%80%E6%B5%8B%E6%A3%80%E6%B5%8B%E6%98%AF%E5%95%A5%E6%B5%8F%E8%A7%88%E5%99%A8)
    - [能力监测](#%E8%83%BD%E5%8A%9B%E7%9B%91%E6%B5%8B)
    - [怪癖检测](#%E6%80%AA%E7%99%96%E6%A3%80%E6%B5%8B)
    - [用户代理检测](#%E7%94%A8%E6%88%B7%E4%BB%A3%E7%90%86%E6%A3%80%E6%B5%8B)
  - [10.DOM](#10DOM)
    - [节点层次](#%E8%8A%82%E7%82%B9%E5%B1%82%E6%AC%A1)
    - [DOM操作技术](#DOM%E6%93%8D%E4%BD%9C%E6%8A%80%E6%9C%AF)
  - [11.DOM拓展](#11DOM%E6%8B%93%E5%B1%95)
    - [选择符API](#%E9%80%89%E6%8B%A9%E7%AC%A6API)
    - [元素遍历](#%E5%85%83%E7%B4%A0%E9%81%8D%E5%8E%86)
    - [HTML5](#HTML5)
    - [专有扩展](#%E4%B8%93%E6%9C%89%E6%89%A9%E5%B1%95)
  - [12.DOM2和DOM3](#12DOM2%E5%92%8CDOM3)
    - [DOM变化](#DOM%E5%8F%98%E5%8C%96)
    - [样式](#%E6%A0%B7%E5%BC%8F)
    - [遍历](#%E9%81%8D%E5%8E%86)
    - [范围](#%E8%8C%83%E5%9B%B4)
  - [13.事件](#13%E4%BA%8B%E4%BB%B6)
    - [事件流](#%E4%BA%8B%E4%BB%B6%E6%B5%81)
    - [事件处理程序](#%E4%BA%8B%E4%BB%B6%E5%A4%84%E7%90%86%E7%A8%8B%E5%BA%8F)
    - [事件对象](#%E4%BA%8B%E4%BB%B6%E5%AF%B9%E8%B1%A1)
    - [事件类型](#%E4%BA%8B%E4%BB%B6%E7%B1%BB%E5%9E%8B)
    - [内存和性能](#%E5%86%85%E5%AD%98%E5%92%8C%E6%80%A7%E8%83%BD)
    - [模拟事件](#%E6%A8%A1%E6%8B%9F%E4%BA%8B%E4%BB%B6)
  - [20.Json](#20Json)
    - [语法](#%E8%AF%AD%E6%B3%95-1)
      - [简单值](#%E7%AE%80%E5%8D%95%E5%80%BC)
      - [对象](#%E5%AF%B9%E8%B1%A1)
      - [数组](#%E6%95%B0%E7%BB%84)
    - [解析与序列化](#%E8%A7%A3%E6%9E%90%E4%B8%8E%E5%BA%8F%E5%88%97%E5%8C%96)
      - [JSON对象](#JSON%E5%AF%B9%E8%B1%A1)
      - [序列化选项](#%E5%BA%8F%E5%88%97%E5%8C%96%E9%80%89%E9%A1%B9)
  - [21.Ajax与Comet](#21Ajax%E4%B8%8EComet)
    - [XMLHttpRequest对象](#XMLHttpRequest%E5%AF%B9%E8%B1%A1)
    - [XMLHttpRequest 2级](#XMLHttpRequest-2%E7%BA%A7)
    - [进度事件](#%E8%BF%9B%E5%BA%A6%E4%BA%8B%E4%BB%B6)
    - [跨域资源共享](#%E8%B7%A8%E5%9F%9F%E8%B5%84%E6%BA%90%E5%85%B1%E4%BA%AB)
    - [其他跨域技术](#%E5%85%B6%E4%BB%96%E8%B7%A8%E5%9F%9F%E6%8A%80%E6%9C%AF)
    - [安全](#%E5%AE%89%E5%85%A8)
  - [22.高级技巧](#22%E9%AB%98%E7%BA%A7%E6%8A%80%E5%B7%A7)
    - [高级函数](#%E9%AB%98%E7%BA%A7%E5%87%BD%E6%95%B0)
    - [防篡改对象](#%E9%98%B2%E7%AF%A1%E6%94%B9%E5%AF%B9%E8%B1%A1)
    - [高级定时器](#%E9%AB%98%E7%BA%A7%E5%AE%9A%E6%97%B6%E5%99%A8)
    - [自定义事件](#%E8%87%AA%E5%AE%9A%E4%B9%89%E4%BA%8B%E4%BB%B6)
    - [拖放](#%E6%8B%96%E6%94%BE)
  - [23.离线应用与客户端存储](#23%E7%A6%BB%E7%BA%BF%E5%BA%94%E7%94%A8%E4%B8%8E%E5%AE%A2%E6%88%B7%E7%AB%AF%E5%AD%98%E5%82%A8)
    - [离线监测](#%E7%A6%BB%E7%BA%BF%E7%9B%91%E6%B5%8B)
    - [应用缓存](#%E5%BA%94%E7%94%A8%E7%BC%93%E5%AD%98)
    - [数据存储](#%E6%95%B0%E6%8D%AE%E5%AD%98%E5%82%A8)
  - [24.最佳实践](#24%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5)
    - [可维护性](#%E5%8F%AF%E7%BB%B4%E6%8A%A4%E6%80%A7)
    - [性能](#%E6%80%A7%E8%83%BD)
    - [部署](#%E9%83%A8%E7%BD%B2)
- [ES6](#ES6)
  - [11.Promise与异步编程](#11Promise%E4%B8%8E%E5%BC%82%E6%AD%A5%E7%BC%96%E7%A8%8B)
    - [异步编程](#%E5%BC%82%E6%AD%A5%E7%BC%96%E7%A8%8B)
    - [Promise基础](#Promise%E5%9F%BA%E7%A1%80)
    - [全局的Promise拒绝处理](#%E5%85%A8%E5%B1%80%E7%9A%84Promise%E6%8B%92%E7%BB%9D%E5%A4%84%E7%90%86)
    - [串联Promise](#%E4%B8%B2%E8%81%94Promise)
    - [响应多个Promise](#%E5%93%8D%E5%BA%94%E5%A4%9A%E4%B8%AAPromise)
    - [自Promise继承](#%E8%87%AAPromise%E7%BB%A7%E6%89%BF)
    - [基于Promise的异步任务执行](#%E5%9F%BA%E4%BA%8EPromise%E7%9A%84%E5%BC%82%E6%AD%A5%E4%BB%BB%E5%8A%A1%E6%89%A7%E8%A1%8C)
- [你不知道的JS](#%E4%BD%A0%E4%B8%8D%E7%9F%A5%E9%81%93%E7%9A%84JS)
  - [作用域和闭包](#%E4%BD%9C%E7%94%A8%E5%9F%9F%E5%92%8C%E9%97%AD%E5%8C%85)
    - [作用域是什么](#%E4%BD%9C%E7%94%A8%E5%9F%9F%E6%98%AF%E4%BB%80%E4%B9%88)
      - [编译原理](#%E7%BC%96%E8%AF%91%E5%8E%9F%E7%90%86)
      - [理解作用域](#%E7%90%86%E8%A7%A3%E4%BD%9C%E7%94%A8%E5%9F%9F)
      - [作用域嵌套](#%E4%BD%9C%E7%94%A8%E5%9F%9F%E5%B5%8C%E5%A5%97)
      - [异常](#%E5%BC%82%E5%B8%B8)
    - [词法作用域](#%E8%AF%8D%E6%B3%95%E4%BD%9C%E7%94%A8%E5%9F%9F)
      - [词法阶段](#%E8%AF%8D%E6%B3%95%E9%98%B6%E6%AE%B5)
      - [欺骗词法](#%E6%AC%BA%E9%AA%97%E8%AF%8D%E6%B3%95)
      - [性能](#%E6%80%A7%E8%83%BD-1)
    - [函数作用域和块作用域](#%E5%87%BD%E6%95%B0%E4%BD%9C%E7%94%A8%E5%9F%9F%E5%92%8C%E5%9D%97%E4%BD%9C%E7%94%A8%E5%9F%9F)
      - [函数中的作用域](#%E5%87%BD%E6%95%B0%E4%B8%AD%E7%9A%84%E4%BD%9C%E7%94%A8%E5%9F%9F)
      - [隐藏内部实现](#%E9%9A%90%E8%97%8F%E5%86%85%E9%83%A8%E5%AE%9E%E7%8E%B0)
      - [函数作用域](#%E5%87%BD%E6%95%B0%E4%BD%9C%E7%94%A8%E5%9F%9F)
      - [块作用域](#%E5%9D%97%E4%BD%9C%E7%94%A8%E5%9F%9F)
    - [提升](#%E6%8F%90%E5%8D%87)
      - [变量声明提升和函数声明提升](#%E5%8F%98%E9%87%8F%E5%A3%B0%E6%98%8E%E6%8F%90%E5%8D%87%E5%92%8C%E5%87%BD%E6%95%B0%E5%A3%B0%E6%98%8E%E6%8F%90%E5%8D%87)
      - [编译器处理提升](#%E7%BC%96%E8%AF%91%E5%99%A8%E5%A4%84%E7%90%86%E6%8F%90%E5%8D%87)
      - [函数优先](#%E5%87%BD%E6%95%B0%E4%BC%98%E5%85%88)
    - [作用域闭包](#%E4%BD%9C%E7%94%A8%E5%9F%9F%E9%97%AD%E5%8C%85)
      - [实质问题](#%E5%AE%9E%E8%B4%A8%E9%97%AE%E9%A2%98)
      - [循环和闭包](#%E5%BE%AA%E7%8E%AF%E5%92%8C%E9%97%AD%E5%8C%85)
      - [模块](#%E6%A8%A1%E5%9D%97)
    - [附录](#%E9%99%84%E5%BD%95)
      - [动态作用域](#%E5%8A%A8%E6%80%81%E4%BD%9C%E7%94%A8%E5%9F%9F)
      - [块级作用域的替代方案](#%E5%9D%97%E7%BA%A7%E4%BD%9C%E7%94%A8%E5%9F%9F%E7%9A%84%E6%9B%BF%E4%BB%A3%E6%96%B9%E6%A1%88)
      - [this词法](#this%E8%AF%8D%E6%B3%95)
  - [this和对象原型](#this%E5%92%8C%E5%AF%B9%E8%B1%A1%E5%8E%9F%E5%9E%8B)
    - [关于this](#%E5%85%B3%E4%BA%8Ethis)
      - [为什么要用this](#%E4%B8%BA%E4%BB%80%E4%B9%88%E8%A6%81%E7%94%A8this)
      - [误解](#%E8%AF%AF%E8%A7%A3)
      - [this到底是什么](#this%E5%88%B0%E5%BA%95%E6%98%AF%E4%BB%80%E4%B9%88)
    - [this全面解析](#this%E5%85%A8%E9%9D%A2%E8%A7%A3%E6%9E%90)
      - [调用位置](#%E8%B0%83%E7%94%A8%E4%BD%8D%E7%BD%AE)
      - [绑定规则](#%E7%BB%91%E5%AE%9A%E8%A7%84%E5%88%99)
      - [优先级](#%E4%BC%98%E5%85%88%E7%BA%A7)
      - [绑定例外](#%E7%BB%91%E5%AE%9A%E4%BE%8B%E5%A4%96)
      - [重提this词法](#%E9%87%8D%E6%8F%90this%E8%AF%8D%E6%B3%95)
    - [对象](#%E5%AF%B9%E8%B1%A1-1)
      - [对象语法](#%E5%AF%B9%E8%B1%A1%E8%AF%AD%E6%B3%95)
      - [对象类型](#%E5%AF%B9%E8%B1%A1%E7%B1%BB%E5%9E%8B)
      - [对象的内容](#%E5%AF%B9%E8%B1%A1%E7%9A%84%E5%86%85%E5%AE%B9)
      - [遍历](#%E9%81%8D%E5%8E%86-1)
    - [混合对象“类”](#%E6%B7%B7%E5%90%88%E5%AF%B9%E8%B1%A1%E7%B1%BB)
      - [类理论](#%E7%B1%BB%E7%90%86%E8%AE%BA)
      - [类的机制](#%E7%B1%BB%E7%9A%84%E6%9C%BA%E5%88%B6)
      - [类的继承](#%E7%B1%BB%E7%9A%84%E7%BB%A7%E6%89%BF)
      - [混入](#%E6%B7%B7%E5%85%A5)
    - [原型](#%E5%8E%9F%E5%9E%8B)
    - [行为委托](#%E8%A1%8C%E4%B8%BA%E5%A7%94%E6%89%98)
    - [ES6中的class](#ES6%E4%B8%AD%E7%9A%84class)
  - [类型和语法](#%E7%B1%BB%E5%9E%8B%E5%92%8C%E8%AF%AD%E6%B3%95)
    - [类型](#%E7%B1%BB%E5%9E%8B)
    - [值](#%E5%80%BC)
    - [原生函数](#%E5%8E%9F%E7%94%9F%E5%87%BD%E6%95%B0)
    - [强制类型转换](#%E5%BC%BA%E5%88%B6%E7%B1%BB%E5%9E%8B%E8%BD%AC%E6%8D%A2)
    - [语法](#%E8%AF%AD%E6%B3%95-2)
    - [混合环境JavaScript](#%E6%B7%B7%E5%90%88%E7%8E%AF%E5%A2%83JavaScript)
  - [异步和性能](#%E5%BC%82%E6%AD%A5%E5%92%8C%E6%80%A7%E8%83%BD)
    - [异步的现在和将来](#%E5%BC%82%E6%AD%A5%E7%9A%84%E7%8E%B0%E5%9C%A8%E5%92%8C%E5%B0%86%E6%9D%A5)
    - [回调](#%E5%9B%9E%E8%B0%83)
    - [Promise](#Promise)
    - [生成器](#%E7%94%9F%E6%88%90%E5%99%A8)
    - [程序性能](#%E7%A8%8B%E5%BA%8F%E6%80%A7%E8%83%BD)
    - [性能测试与调优](#%E6%80%A7%E8%83%BD%E6%B5%8B%E8%AF%95%E4%B8%8E%E8%B0%83%E4%BC%98)
    - [asynquence库](#asynquence%E5%BA%93)
    - [高级异步模式](#%E9%AB%98%E7%BA%A7%E5%BC%82%E6%AD%A5%E6%A8%A1%E5%BC%8F)
  - [起步上路](#%E8%B5%B7%E6%AD%A5%E4%B8%8A%E8%B7%AF)
    - [深入编程](#%E6%B7%B1%E5%85%A5%E7%BC%96%E7%A8%8B)
    - [深入JavaScript](#%E6%B7%B1%E5%85%A5JavaScript)
  - [ES6及更新版本](#ES6%E5%8F%8A%E6%9B%B4%E6%96%B0%E7%89%88%E6%9C%AC)
    - [ES的现在与未来](#ES%E7%9A%84%E7%8E%B0%E5%9C%A8%E4%B8%8E%E6%9C%AA%E6%9D%A5)
    - [ES6语法](#ES6%E8%AF%AD%E6%B3%95)
    - [代码组织](#%E4%BB%A3%E7%A0%81%E7%BB%84%E7%BB%87)
    - [异步流控制](#%E5%BC%82%E6%AD%A5%E6%B5%81%E6%8E%A7%E5%88%B6)
    - [集合](#%E9%9B%86%E5%90%88)
    - [新增API](#%E6%96%B0%E5%A2%9EAPI)
    - [元编程](#%E5%85%83%E7%BC%96%E7%A8%8B)
    - [ES6之后](#ES6%E4%B9%8B%E5%90%8E)

# JS高程
## 1.JavaScript简介
### JavaScript简史
### JavaScript实现
- ES
- DOM
- BOM
### JavaScript版本

## 2.在HTML中使用JavaScript
### script元素
- 标签的位置
- 延迟脚本
- 异步脚本
- 在XHTML中的用法
- 不推荐使用的语法
### 嵌入代码与外部文件
### 文档模式
### noscript元素

## 3.基础概念
### 语法
- 区分大小写
- 标识符
- 注释
- 严格模式
- 语句
### 关键字和保留字
### 变量
### 数据类型
- typeof操作符
  - 用来检测变量的数据类型
  - `typeof null //object`
  - `typeof (new RegExp())  //object,chrome7之前返回function`
  - `typeof()可以使用，但不必要，typeof是操作符不是函数`
- Undefined类型
  - undefined类型只有一个值`undefined`
  - 声明变量但未初始化会默认为变量赋值`undefined`，只要值是`undefined`，他的`typeof`就是`undefined`
  - 未声明的变量只能执行一项操作`typeof`，结果为`undefined`，也可以执行delete，但无意义
- Null类型
  - null类型只有一个值`null`，表示一个空对象指针
  - undefined == null //true
  - 在还不知道为一个变量声明时初始化什么值时，可以初始化为null
  - null和undefined本质上是不同的，语义不同
- Boolean类型
  - 只有`true`和`false`两个值
  - 所有类型的值都有与这两个布尔值等价的值，可以通过`Boolean()`转换，任何类型都可以调用这个函数
  - 转换规则
    |数据类型|true|false|
    |:--:|:--:|:--:|
    |String|任何非空字符串|""（空字符串）|
    |Number|任何非零数值(包括无穷大)|0和NaN|
    |Object|任何对象|null|
    |Undefined|N/A|undefined|
  - 流控制语句自动执行相应的布尔转换 
- Number类型
  - 使用IEEE754格式表示整数和字符串
  - 数值字面量格式
    - 八进制：0开头，每位在0-7之间，否则按十进制解析
    - 十六进制：0x开头，每位在0-9，A-F之间，否则报错
    - +0 == -0 //true
    - 十进制：默认
  - 浮点数值
    - `.0 == 0.1`
    - `1. == 1`浮点数占空间是数值的两倍，所以会最大程度的把浮点数转换成整数
    - `1.0 == 1`浮点数本身是整数会被转换成整数
    - `e`科学计数法
    - 浮点数的最高精度是17位，所以0.1+0.2=0.30000000000000004(15个0，小数点后17位)
  - 数值范围
    - Number.MIN_VALUE: 5e-324
      - `Number.MIN_VALUE - Number.MIN_VALUE == 0`
      - `Number.MIN_VALUE - Number.MAX_VALUE == - Number.MAX_VALUE`
      - `Number.MIN_VALUE + Number.MIN_VALUE == 1e-323`
      - `Number.MIN_VALUE + Number.MAX_VALUE == Number.MAX_VALUE`
      - `Number.MIN_VALUE + 任何非零数 == 该非零数`
    - Number.MAX_VALUE: 1.7976931348623157e+308
      - `Number.MAX_VALUE - Number.MAX_VALUE == 0`
      - `Number.MAX_VALUE - Number.MIN_VALUE == Number.MAX_VALUE`
      - `Number.MAX_VALUE + Number.MAX_VALUE == Infinite`
      - `Number.MAX_VALUE + Number.MIN_VALUE == Number.MAX_VALUE`
      - `Number.MIN_VALUE + 任何非零数 == Number.MAX_VALUE
    - Number.NEGATIVE_INFINITE: -Infinite
      - `Number.NEGATIVE_INFINITE + Number.POSITIVE_INFINITE == NaN`
    - Number.POSITIVE_INFINITE: Infinite
    - isFinite()：用来检查数值是否有限
  - NaN
    - Not a Number,表示本来要返回数值的操作数未返回数值，是一个特殊的数值
    - 任何涉及NaN的操作都会返回NaN
    - NaN与任何值都不相等`NaN == NaN //false`
    - isNaN(),传入所有不能转换成数值的值和NaN会返回true
  - 数值转换
    - 三个函数可以把非数值转成数值：`Number()`、`parseInt()`、`parseFloat()`
    - Number()
      - 传入布尔，1和0
      - 传入数值，根据数值格式输出数值
      - 传入null，返回0
      - 传入undefined，返回NaN
      - 传入字符串
        - 字符串中只包含数值和无意义的空格，返回数值的十进制
        - 字符串中包含有效浮点格式，返回对应的浮点数值
        - 字符串以0x开头的有效十六进制格式，返回对应的十进制整数
        - 字符串为空，返回0
        - 字符串中包含其他字符，返回NaN
      - 传入对象
        - 首先调用对象的`ValueOf()`方法，然后依照前面的规则转换返回值，如果结果是NaN，则调用对象的`toString()`方法，然后依照前面的规则转换返回的字符串
      - Number()与一元加操作符的操作相同，即`+true == 1`
    - parseInt() 
      - 会忽略字符串前面的空格，知道找到第一个非空格字符，若第一个字符不是数字或符号，则返回NaN
        - parseInt("   1") == Number("   1")
      - 会一直解析直到遇到非数值
        - parseInt("1.2") == 1
        - parseInt("123bl") == 123
        - parseInt("0x) == NaN
      - 第二个参数，传入基数表示数字格式
        - parseInt("70",8) //56 ，可忽略0开头
        - 建议无论在何时都传入基数，默认10
    - parseFloat()
      - 解析直到第一个无效浮点数字符，可返回整数
      - 没有第二个参数
        - 传入十六进制，返回0，因为到x就认定无效了
        - 当有效数字不止一个0的时候忽略前置0，只解析十进制
- String类型
  - 由0或多个16位Unicode字符组成的字符序列，用`""`或`''`表示
  - 字符字面量
    - 转义序列
      - `\n` ：n表示newline，换行
      - `\t` ：t表示table，就是一个tab的缩进
      - `\b` ：b表示backspace，就是退格
      - `\r` ：r表示return，回车
      - `\f` ：f表示formfeed，进纸
      - `\\` ：斜杠
      - `\'` ：单引号
      - `\"` ：双引号
      - `\xnn` ：n表示十六进制，表示一个字符
        - \x41 : A
      - `\unnnn` ：n表示十六进制，表示一个Unicode字符，六个字符长，表示一个字符
        - \u03a3 : sigma
        - '\u03a3'.lenght == 1
    - 字符长度
      - 转义序列无论多长，只占一位
  - 字符串特点
    - 字符串一旦创建就不可改变
    - 要改变保存字符串的变量，直接将变量指向一个新字符串，旧的字符串会被销毁
  - 转换为字符串
    - 两种方式把一个值转为字符串：`toString()`和`String()`
    - toString()
      - 数值、字符串、对象、布尔值都有toString()方法
        - null和undefined没有
        - 字符串也有，返回该字符串的一个副本
      - 传参
        - 数值调用toString()时，传入一个基数，来表示数值转换的进制数，默认十进制
        - `var a = 10 ; a.toString(2) //"1010"`
    - String()
      - 能将任何类型的值转换为字符串
      - 转换规则
        - 如果值由toString()方法，则调用该方法，不传参
        - 如果值是null，返回'null'
        - 如果值是undefined，返回'undefined'
    - 数字转字符串简单方法
      - `num + ""`
    - 纯数字的字符串转数字
      - `+str`
- Object类型
  - 一组数据和功能的集合
  - 每个对象实例都具有的属性和方法
    - `constructor`
    - `hasOwnProperty(prototypeName)`
    - `isPrototypeOf(object)`
    - `prototypeIsEnumberable(prototypeName)`
    - `toLocalString()`返回对象的字符串表示，跟执行环境相关
    - `toString()`返回对象的字符串表示。`￥￥￥`
    - `valueOf()`
### 操作符
>主要分四大类：算数运算符、位运算符、关系操作符、相等操作符
<br>ES中的操作符不同之处在于能够适用于多种类型的值，在应用对象时，会调用对象的valueOf或toString

- 一元操作符：只能操作一个值的操作符
  - 递增和递减操作符
    - `a++\++a`
    - `a--\--a`
  - 一元加和一元减操作符
    - `+num`
    - `-num`
- 位操作符
  - 二进制补码
    - 传统三步法
      - 绝对值的二进制码
      - 反码
      - 反码+1
    - JavaScript输出负数
      - 绝对值的二进制码
      - 前面加个负号
  - 位操作符
    - ES中对数值使用位操作符会将64位的数值转换成32位，进行位运算，最后转换回64位
    - NaN和Infinity被当做0来处理，对非数值进行位运算会先进行Number()chuli 
  - 按位非(NOT) `~`
    - `num == - ( ~ num + 1)`
  - 按位与(AND) `&`
  - 按位或(OR) `|`
  - 按位异或(XOR) `^`
    - `(num1 ^ num2) == (num1 | num2) - (num1 & num2)`
  - 左移 `<<`
    - 所有位数左移，腾出的空位用0补充，不会影响符号位，除非移到了第32位，超出32位为0
  - 有符号的右移 `>>`
    - 符号位不动，其他位右移，腾出位用符号位的值来填充(负数用1填充，正数用0填充)
  - 无符号的右移 `>>>`
    - 32位整体右移
    - 正数，与>>相同
    - 负数，腾出位用0填充
- 布尔操作符
  - 逻辑非 `!`
  - 逻辑与 `&&`
  - 逻辑或 `||`
- 乘性操作符
  - 乘法 `*`
  - 除法 `/`
  - 求模 `%`
- 加性操作符
  - 加法 `+`
  - 减法 `-`
- 关系操作符
  - 小于 `<`
  - 大于 `>`
  - 小于等于 `<=`
  - 大于等于 `>=`
- 相等操作符
  - 相等 `==`
  - 不相等 `!=`
  - 全等 `===`
  - 不全等 `!==`
- 条件操作符
  - 问号 `a?b:c`
- 赋值操作符
  - 等号 `=`
- 逗号操作符
  - 用于赋值 `var a = (5, 1, 4)`，用于赋值时，逗号操作符会返回表达式中的最后一项
  - 用于声明 `var a = 1, b = 2`
### 语句
- if语句
- do-while语句
- while语句
- for语句
- for-in语句
- label语句
- break和continue语句
- with语句
- switch语句
### 函数
- 理解参数
  - arguments对象
    - 是一个类数组，不是Array的实例
      - arguments[],可以为空，所以ES的函数参数非必要
      - arguments.length
- 没有重载
  - 后面的声明会覆盖前面的声明

## 4.变量、作用域和内存问题
### 基本类型和引用类型的值

- 变量的访问
    + 基本类型 **按值访问**，可以操作保存在变量中的实际的值
    + 引用类型 **按引用访问**，实际的值是保存在内存中的对象，不能直接操作对象的内存空间。在为对象添加属性时，操作的是实际的对象，在复制保存着对象的某个变量时，操作的是对象的引用
- 动态的属性
    + 引用类型可以动态的操作属性
- 复制变量值
    + 基本类型复制的是值，两个值相同但互不相干
    + 引用类型复制的是指针，两个指针指向内存空间中同一个对象
- 传递参数
    + 无论传参是基本类型还是引用类型，**都是按值传递**
    + 参数实际上是函数的局部变量，用ES的概念说，是arguments对象中的一个元素
    + 在函数内部重写一个全局对象时，这个之前的全局对象会变成一个局部对象，局部对象会在函数执行完毕后立即销毁
- 检测类型
    + `typeof`方便检测基本类型
    + `instanceof`方便检测引用类型


### 执行环境及作用域
- 产生：当某个函数被调用时，会创建一个执行环境及相应的作用域链，然后用arguments和其他命名参数的值来初始化活动对象
- 执行环境：`execution context`也叫执行上下文，定义了变量或函数有权访问的其他数据，决定了它们各自的行为
    + 变量对象：环境中定义的所有变量和函数都保存在这个对象中。解析器在处理数据时会在后台使用这个对象,编码过程中无法访问这个对象
    + 全局执行环境：最外围的一个执行环境，在web浏览器中，全局执行环境是window对象，因此所有的全局变量和函数都是作为window对象的属性和方法创建的
    + 环境的销毁：某个执行环境中所有代码执行完毕后，该环境被销毁，保存在其中的所有变量和属性定义也随之销毁。全局执行环境直到应用程序退出时才被销毁
    + 执行流：每个函数都有自己的执行环境，当执行流进入一个函数时，函数的环境被推入一个环境栈中。在函数执行之后，栈将其环境弹出，把控制权返回给之前的执行环境
- 作用域链：指向变量对象的指针列表，只引用但不实际包含变量对象。保证对执行环境有权访问的所有变量和函数的有序访问
    + 作用域链的前端：始终都是当前执行的代码所在环境的变量对象
        * 如果执行环境是函数，将其 **活动对象**作为变量对象。活动对象最开始只包含arguments对象一个变量
    + 作用域链的最后端：始终都是全局执行环境的变量对象
    + 中间：下一个变量对象来自下一个包含(外部)环境，直至延续到全局执行环境
    + 标识符解析：沿着作用域链一级一级地搜索标识符的过程
- 延长作用域链
    + try-catch语句
    + with语句

- 没有块级作用域
    + es6补充let、const关键字


### 垃圾收集
- 原理：找出不再使用的变量(打上记号)，然后周期性地释放其占用的内存。
- 标记清除(最主流)
  - 当变量进入环境时，为这个变量标记为“进入环境”，当变量离开环境时，则将其标记为“离开环境”
  - 如何标记不重要，关键在于采取什么策略
  - 垃圾收集器工作
    - 给存储在内存中的所有变量加上标记(加上进入环境的标签)
    - 去掉环境中的变量以及被环境中变量引用的变量的标记(摘掉进入环境的标签)
    - 环境中无法访问的变量加上标签(加上离开环境的标签)
    - 内存清除，销毁哪些带标签的值并回收他们所占用的内存空间
- 引用计数
  - 原理：跟踪记录每个值被引用的次数
  - 步骤：
    - 变量被声明时并被赋值一个引用类型值时，+1，该引用类型被赋值给另一个变量，+1
    - 包含这个引用的变量又取得另一个值，-1，
    - 当引用次数为0时，则可以销毁了
  - 引用计数的问题
    - 循环引用会导致次数永不为0，例如IE的DOM
  - 手动解决方案
    - 为了避免循环引用，赋值为null，手动解除引用
  - 内存泄露
    - 使用引用计数的垃圾清理机制会存在的问题，就是已经不再用到的内存，没有及时释放(次数不为0)
- 性能问题
  - IE是通过动态修改几个字面量的临界值的方式来触发垃圾收集器
    - 256个变量
    - 4096个对象
    - 64kb字符串
    - 触发任一临界值便会触发，定死临界值可能会频繁触发回收。所以需要动态修改临界值
  - 当垃圾收集例程回收的内存分配量低于15%(每次回收的内存占比不大，说明总是被清除)，上面的临界值加倍
  - 当垃圾收集例程回收的内存分配量达到85%(每次回收的内存占比大，说明很久没被清除)，临界值重置默认值
- 管理内存
  - 一旦数据不再有用，最好通过设置为null来释放引用，这个方法叫解除引用
    - **解除引用**并不是直接释放内存，而是方便垃圾收集器下次运行时将他带走
  - 局部变量会在他们离开执行环境时自动被解除引用

## 5.引用类型
- 引用类型是一种数据结构，用于将数据和功能组织到一起。比如Array.push()，Array是数组，push是为数组增加元素的功能。
- 引用类型也是一种对象定义，描述一类对象所具有的的属性和方法
- 引用类型和类不是相同的概念，对象是引用类型的实例

### Object类型

### Array类型
- 检测数组
  - instanceof操作符
  - Array.isArray(value)
- 转换方法
  - toString()
  - toLocalString()
  - valueOf()
- 栈方法
  - push()
  - pop()
- 队列方法
  - push()和shift()
  - unshift()和pop()
- 重排序方法
  - reverse()
  - sort()
- 操作方法
  - concat
  - slice
  - splice
- 位置方法
  - indexOf
  - lastIndexOf
- 迭代方法
  - every
  - filter
  - forEach
  - map
  - some
- 归并方法
  - reduce
  - reduceRight
### Date类型
### RegExp类型
- 格式：`var expression = / pattern / flags ;`
  - pattern表示正则表达式
  - flags表示标志
    - g：表示全局模式，即正则应用到字符串全局，并非第一个处
    - i：表示不区分大小写模式
    - m：表示多行模式
- RegExp构造函数
  - 两个参数
    - 字符串模式
      - 需要双重转义
    - 标志字符串
### Function类型
### 基本包装类型
### 单体内置对象

## 6.面向对象的程序设计

### 理解对象
- 属性类型：为了实现JavaScript引擎，在JavaScript中不能直接访问它们
    + 数据属性：包含一个数据值的位置，在这个位置可以读写值，有4个描述行为特性的描述符
        * `[[Configurable]]`表示能否通过delete删除属性从而重新定义属性，能否修改属性的特性、能否把属性修改为访问器属性
            - 一旦把属性定义为不可配置的，就不能再把它变回可配置的了
        * `[[Enumerable]]`表示能否通过for——in循环返回属性
        * `[[writable]]`表示能否修改属性的值
        * `[[value]]`表示这个属性的数据值
    + 访问器属性：不包含数据值，包含一对getter和setter函数(非必需)
        * 不能直接定义，必须使用defineProperty来定义
        * `[[Configurable]]`同上
        * `[[Enumerable]]`同上
        * `[[Get]]`在读取属性时调用的函数。默认值undefined
        * `[[Set]]`在写入属性时调用的函数。默认值undefined
        * 使用方式同数据属性，使用访问器属性的常见方式是设置一个属性的值会导致其他属性发生变化。
    + `Object.defineProperty()`:修改一个属性默认的特性
        * 接受三个参数：属性所在对象，属性名，一个描述符对象
        * 描述符对象的属性为：configurable、enumerable、writable、value
- 定义多个属性：`Object.defineProperties()`
    + 接收两个参数:属性所在对象，属性名和描述符对象的键值对对象
    + 所有的属性都是在同一时间创建的
- 读取属性的特性:`Object.getOwnPropertyDescriptor()`
    + 接收两个参数：属性所在对象、要读取其描述符的属性名
    + 返回值是一个对象，对象的属性视数据属性和访问器属性而不同


### 创建对象
- 工厂模式
    + 用简单的函数创建对象，为对象添加属性和方法，然后返回对象
    + 基本思路：抽象创建具体对象的过程，封装以特定接口创建对象的细节
- 构造函数模式
    + 创建自定义引用类型，像创建内置对象实例一样使用new操作符创建引用类型实例
    + 和工厂模式的区别
        * 没有显式的创建对象 `new Object()`
        * 直接将属性和方法赋给了`this`对象
        * 构造函数没有`return`语句
    + 用 `new` 构造函数创建实例，会经历4个步骤
        * 创建一个新对象
        * 将构造函数的作用域赋给新对象(为了this指向新对象)
        * 执行构造函数中的代码
        * 返回新对象
    + `实例名.constructor == 构造函数名      //true`
    + `实例名 instanceof 构造函数名/Object   //true`
    + 问题：每个方法都要在每个实例上重新创建一遍
        * `person1.方法 == person2.方法    //false`
        * 可以把方法的定义转移到构造函数外部，而在构造函数内部，将方法属性设置成等于这个全局方法(保存指向这个全局方法的指针)
            - 这样做多了就会使封装性减弱
- 原型模式
    + 基本思路：使用构造函数的`prototype`属性来指定哪些应该共享的属性和方法
        * 创建的每一个函数都有一个`prototype`属性，保存着指向一个对象的指针，这个对象的用途是包含所有实例 **可共享**的属性和方法。
        * `prototype`是通过调用构造函数而创建的那个实例的原型对象，可以不必在构造函数中定义对象实例的信息
    + **原型对象**
        * `Function.prototype`:每创建一个函数，就会创建一个prototype属性，该属性指向函数的原型对象
        * `Function.prototype.constructor`:所有的原型对象会自动获取一个constructor属性，指向prototype属性所在函数
            - `Person.prototype.constructor == Person`
        * `实例.__proto__`:当调用构造函数创建一个实例后，这个实例中会包含一个指向构造函数原型对象的指针`[[prototype]]`，在浏览器上是的体现是每个实例对象上有一个 `__proto__`属性
        * 总结：实例的属性中会有`__proto__`属性指向原型对象，构造函数中会有`prototype`属性指向原型对象，原型对象中会有`constructor`属性指向构造函数
        * `isPrototypeOf()`
            - `Person.prototype.isPrototypeOf(person1) //true`
        * `Object.getPrototypeOf()`
            - `Object.getPrototypeOf(person1) == Person.prototype //true`
        * 原型搜索机制
            - 原理：对象实例共享原型所保存的属性和方法
            - 当读取某个对象的某个属性时
                + 首先会搜索对象实例本身，如果找到给定的属性或方法名，则返回
                + 若没找到，则对对象实例的原型对象进行第二次搜索，如果找到，则返回
        * `hasOwnProperty()`：检测一个属性是在实例中还是在原型中。该方法继承自Object
            - `person1.hasOwnProperty("name")    //false  表示属性在原型中`
    + 原型与in操作符
        * `in`：无论是实例本身还是原型的属性，只要能访问就为true
            - `"name" in person  //true`
        * `for-in`:返回的是所有可通过对象访问的，enumerated的属性
            - 包括存在于实例的属性，也包括存在与原型的属性
            - 会屏蔽原型中不可枚举的属性(即[[enumerable]]设置为false的属性)，但实例属性覆盖该原型属性后是可以的
            - 所有开发人员定义的属性都是可枚举的 
        * `Object.keys(原型对象)`:返回一个所有可枚举属性的字符串数组
            - `Object.keys(Person.prototype)     //name,age,job,sayName`
        * `Object.getOwnPropertyNames(原型对象)`：返回所有属性的字符串数组
            - `Object.getOwnPropertyNames(Person.prototype)  //constructor,name,age,job,sayName`
    + 对象字面量方式重写原型对象
        * 重写原型就切断了现有实例与新原型的联系
        * 新原型的`constructor`不再指向`Person`,而是`Object`。因为重写了原型对象，这个原型就是Object的实例，它的constructor属性也就指向了最顶层Object
            - `person1 instanceof Person `//true
            - `person1.constructor == Person `//false
        * 解决方法
            - 对象字面量中加一条`constructor : Person,`。但是会产生一个新的问题：constructor变成可枚举的属性。
            - `Object.defineProperty`
            ```javascript
            Object.defineProperty(Person.prototype, "constructor", {
                enumerable : fasle,
                value : Person
             });
            ```
    + 原型的动态性
        * 在通过构造函数创建实例之后修改原型对象
            - 对原型对象内部做任何修改都能够立即从实例上反映出来
            - 如果修改的是整个原型对象，则不具有动态性
                + 重写原型就切断了原本原型和构造函数之间的联系。
                + 此时构造函数的prototype属性指向重写后的原型。
                + 而先前创建的实例中的指针仅指向重写前的原型，而不指向重写后的原型
    + 原生对象的原型
        * 原生引用类型(Object、Array、String等)都在其构造函数的原型上定义了方法
        * 不推荐在原生对象的原型上定义新方法
    + 原型对象的问题
        * 在修改基本类型的属性时，问题不大，因为同名属性会直接覆盖
        * 在修改包含引用类型值的属性时，问题很大，所有实例中的属性都会做出修改
- 组合使用构造函数模式和原型模式
    + 构造函数模式用于定义实例属性，原型模式用于定义方法和共享属性
    + 优点：
        * 支持向构造函数传递参数
        * 每个实例都会有自己的一份实例属性副本
        * 共享着方法的引用，最大限度节省内存
- 动态原型模式
    + 把所有信息都封装在构造函数中，而仅在必要的情况下(第一次被调用时)通过在构造函数中初始化原型
    ```javascript
    if (typeof this.sayName != "Function"){//语句检查可以是任何属性或方法
        Person.prototype.sayName = Function(){//不要用对象字面量方式重写原型对象
            return this.name;
        }
    }
    ```

- 寄生构造函数模式
    + 类似工厂模式：除了使用new操作符和把包装函数称之为构造函数之外和工厂模式一模一样
    + 优点 
        * 可以重写调用构造函数时return的值。普通构造函数只能返回新对象实例
        * 可以用来创建有额外方法的引用类型，如创建一个类似Array的构造函数
    + 缺点
        * 顾名思义，寄生。返回的对象与构造函数和构造函数的原型之间没有关系
    + 不推荐
- 稳妥构造函数模式
    + 稳妥对象：没有公共属性，其方法不引用this关键字
    + 适用于不允许使用this和new的安全环境中
    + 类似寄生构造函数模式;与寄生构造函数模式的区别：
        * 新创建对象的实例方法不引用this
        * 不使用new操作符调用构造函数

### 继承
- 原型链:实现继承的主要方法
    + 基本思路：利用原型让一个引用类型继承另一个引用类型的属性和方法
    + 原型搜索机制拓展：搜索子对象实例->搜索子对象原型->搜索超对象原型直至找到为止
    + `Object.prototype`:默认的原型。原型链的最顶层
        * 所有引用类型默认都继承了Object
        * 所有函数的默认原型都是Object的实例 `Function.prototype = new Object()` 
    + `instanceof`：确定原型和实例的关系，子实例是原型链中任何一个类型的实例
    + `isPrototypeOf()`同`instanceof`
    + 给原型添加方法的代码一定要放在替换原型的语句之后
    + 通过原型链实现继承时，不能使用对象字面量创建原型方法，字面量添加新方法会破坏继承
    + 原型链的问题
        * 通过原型链来实现继承时，原型会变成另一个类型的实例。原先的实例属性就变成了原型属性，即会被共享
        * 创建子类型的实例时，不能向超类型的构造函数中单独传递参数
- 借用构造函数(伪造对象或经典继承)技术
    + 基本思路：在子类型构造函数内部调用超类型的构造函数
    + 实现：通过使用`apply`和`call`方法在将来新创建的对象上执行构造函数
    + 传递参数
        * `superType.call(this,arg1,arg2)`
        * `superType.apply(this,[arg1,arg2])`     
    + 借用构造函数的问题
        * 函数复用率低
- 组合继承(伪经典继承)：将原型链和借用构造函数的技术组合到一块
    + 基本思路：使用原型链实现对原型属性和方法的继承，通过借用构造函数来实现对实例属性的继承
    + 是JavaScript最常用的继承模式
    + 组合继承的问题：每次都会调用两次超类型的构造函数，继承两次实例属性
        * 一次是创建子类型原型时继承实例属性
        * 一次是在子类型构造函数内部继承实例属性
- 原型式继承
    + 基本思路：借助原型基于 **已有的对象**创建新对象(克隆)
    ```JavaScript
    function object(o){
        function F(){}      //新建一个临时性的构造函数
        F.prototype = o;    //将传入的对象作为这个构造函数的原型对象，这里只是浅复制了传入对象o的指针。意思就是这个对象o是外部共享的
        return new F();     //返回这个构造函数的新实例
    }
    ```
    + `Object.create()`:ES5新增用来规范化原型式继承，接受两个参数
        * 用作新对象原型的对象
        * (可选)为新对象定义额外属性的对象
    + 使用场景：想让一个对象和另一个对象保持类似时
- 寄生式继承
    + 基本思路：和寄生构造函数和工厂模式类似，创建一个仅用于封装继承过程的函数
    ```JavaScript
    function createAnother(origObj){
        var cloneObj = object(origObj);
        cloneObj.sayHi = function(){
            console.log("hi");
        };
        return cloneObj
    }
    ```
    + 使用场景：主要考虑的是对象而不是自定义类型和构造函数时
- 寄生组合式继承
    + 基本思路：通过借用构造函数来继承属性，通过原型链的混成形式来继承方法，直接将超类型的原型赋值给子类型的原型，而不是将超类型的实例赋值给子类型原型
    ```JavaScript
    function inheirtPrototype(SubType, SuperType){
        var cloneSuperPrototype = create(SuperType.prototype);//创建对象
        cloneSuperPrototype.contructor = SubType;   //增强对象
        SubType.prototype = cloneSuperPrototype;    //指定对象
    }
    ```
    + 最理想的继承范式

## 7.函数表达式
- 定义函数
    + 函数声明
        * FSCO四大浏览器定义了name属性 `fun.name == 'fun'`
        * 函数声明提升：执行代码之前会先读取函数声明，可以把函数声明放在函数调用之后
    + 函数表达式
        * 创建一个匿名函数(拉姆达函数)赋值给一个变量，匿名函数的name为空字符串`''`
        * 和其他表达式一样，使用前必须先赋值，不存在变量提升
    + 命名函数表达式
        * 严格模式下，不能通过脚本访问arguments.callee时，可在递归函数中使用
        ```JavaScript
        "use strict"
        var factorial = (
            function f(n){
                ...
                return n * f(n-1);
            }
        )
        ```
        * 将函数赋值给另一个变量，函数名字f仍然有效。在严格模式和非严格模式都可以
        * 此时name属性指向f而不是factorial

### 递归
- 递归函数是一个通过名字调用自身的函数
- 通过名字递归的问题
    ```JavaScript
    var anotherFactorial = factorial;   //factorial为递归方法实现的阶乘函数
    factorial = null;
    anotherFactorial(4);    //此时函数内部的facotorial(3)已经不再能执行了
    ```
- `arguments.callee`：一个指向正在执行的函数的指针
- 严格模式下，使用命名函数表示来达成相同的效果

### 闭包
- 作用域链：指向变量对象的指针列表，只引用但不实际包含变量对象。保证对执行环境有权访问的所有变量和函数的有序访问
    + 作用域链的前端：始终都是当前执行的代码所在环境的变量对象
        * 如果执行环境是函数，将其 **活动对象**作为变量对象。活动对象最开始只包含arguments对象一个变量
    + 作用域链的最后端：始终都是全局执行环境的变量对象
    + 中间：下一个变量对象来自下一个外部环境，直至延续到全局执行环境
    + 标识符解析：沿着作用域链一级一级地搜索标识符的过程
- 函数的生命周期
    + 创建函数时，会创建一个预先包含全局变量对象的 **作用域链**，这个作用域链被保存在内部的`[[scope]]`属性中
    + 调用函数时
        * 自动取得两个特殊变量`this`和`arguments`
        * 会为函数创建一个 **执行环境**，然后通过复制函数的`[[scope]]`属性中的对象构建起执行环境的作用域链。
        * 函数的活动对象被创建并被推入执行环境作用域链的前端
    + 访问函数中的变量时，从作用域链中搜索相应名字的变量
    + 函数执行完毕后，局部活动对象就会被销毁，内存中仅保存全局作用域(全局执行环境的变量对象)
- 闭包:指有权访问另一个函数作用域中的变量的函数(内部函数是其包含函数的闭包)
    + 闭包会携带包含函数的作用域(内存中存储包含函数的变量对象)和全局作用域，会比其他函数占用更多内存
    + 闭包的作用
        * 在JavaScript中模仿块级作用域
        * 用以在对象中创建私有变量(闭包实现能够访问包含作用于中变量的公有方法)
- 闭包与变量
    + 闭包只能取得包含函数中任何变量的最后一个值(在循环中的闭包要注意)
- this对象：基于函数运行时环境绑定的
    + 全局函数中，this等于window
    + 当函数作为对象的方法调用时，this等于那个对象
    + 匿名函数的this指向window，因为匿名函数是全局执行环境
    ```JavaScript
    var name = "window"
    var obj = {
        name:'obj',
        getName:function() {    
            return this.name
        }
    }
    ```
    `obj.getName() `//obj
    `(obj.getName)() `//obj，因为obj.getName和(obj.getName)定义一样
    `(obj.getName = obj.getName)()`//window ,因为赋值表达式的值是匿名函数本身
- 内存泄露
    + 闭包作用域链中不要保存HTML元素，不然该元素无法被销毁
    + 闭包会引用包含函数的整个活动对象
    + 在用完一个变量后，把它设为null
     ```JavaScript
     var element = document.getElementById("x");
     var id = element.id
     element.onclick = function(){
            alert(id)
     }
     element = null //解除对DOM对象的引用
     ```

### 模仿块级作用域
- JavaScript没有块级作用域的概念
    + 变量提升
    ```JavaScript
    var name = 'jimmy'
    function a(){
    console.log(name)
    if(false){
        var name = 'lzm'
    }
    }
    a() //undefined
    ```
    + for循环：
        * i在循环结束后还会存在，因为i定义在for循环的包含函数的活动对象中
        * 即使在循环结束后重新声明i(var i)也没用，因为前面的i还在，会无视后续的声明
- 匿名函数用作块级作用域(私有作用域)
    ```JavaScript
    (function(){
        //这是块级作用域，ES6后被let\const取代
    })()//函数表达式之后才能跟圆括号，比如f()
    ```
    + 匿名函数放在圆括号里，表示是一个函数表达式；之后的圆括号表示会立刻调用这个函数
    + 这个匿名函数被用作块级作用域时会是一个闭包
    + 这种用法可以减少闭包占用的内存问题，因为没有指向匿名函数的引用

### 私有变量
- 任何函数中定义的变量，都可以认为是私有变量。私有变量包含函数的参数、局部变量、函数内部定义的其他函数
- 公有方法：可以访问包含作用于中定义的变量的方法
- 特权方法：是闭包，有权访问私有变量和私有函数的公有方法
    + 在构造函数中定义特权方法
    + 静态私有变量：通过私有作用域中定义私有变量或函数创建特权方法
        * 函数声明只能创建局部函数
        * 非严格模式下，初始化未经声明的变量,总是会创建一个全局变量
    + 多查找作用域中的一个层次，就会在一定程度上影响查找速度。这正是使用闭包和私有变量的一个不足之处
- 模块模式
    + 单例特权方法
- 增强的模块模式

## 8.BOM
- ES是JavaScript的核心，BOM是web环境下JavaScript的核心
- BOM提供了很多对象，用于访问浏览器的功能。这些功能与页面内容无关

### Window对象
- 概念
    + window对象是BOM的核心对象,表示浏览器的实例
    + 两个角色：访问浏览器窗口的JSAPI;ES中的Global对象
- 全局作用域
    + window对象扮演中ES中Global对象的角色
    + `var a` 和 `window.a` 的区别
        * `var`语句声明的全局变量不能通过delete操作符删除。因为使用`var`语句添加的`winodw`属性有一个名为`[[configurable]]`的特性，这个特性值被设置为false
    + 尝试访问未声明的变量会抛错，这时可以通过`window.unknowValue`查看该变量是否存在,未声明则值为undefined.
- 窗口关系及框架
    + `<frame>`标签已被新标准废弃，使用 `<iframe>`
    + 使用框架会使浏览器存在多个Global对象
    + `top`指向最高层的frame,即浏览器窗口window
    + `parent`指向当前frame的上层frame
    + `window == self`引入`self`是为了和`top`、`parent`对应起来
- 窗口位置
    + `screenLeft`/`screenTop`IE、Safari、Opera、Chrome
    + `screenX`/`screenY`FireFox、Safari、Chrome
    + 跨浏览器取的窗口位置
    ```javascript
        var winPosLeft = (typeof window.screenLeft == 'number') ? 
                            window.screenLeft : window.screenX;
        var winPosTop = (typeof window.screenTop == 'number') ? 
                            window.screenTop : window.screenY;
    ```
    + `moveTo(0,100)`窗口移动到新位置的xy值
    + `moveBy(0,100)`窗口向水平和垂直方向移动的像素值
        * 默认被禁用，不适用于frame，只能对最外层window对象使用
- 窗口大小
    + 浏览器窗口内容区域宽高，包括水平/垂直滚动条(如果有的话)
        * `innerWidth`
        * `innerHeight`
    + 浏览器窗口的宽高
        * `onnerWidth`
        * `onnerHeight`
    + `document.documentElement.clientWidth`(后面补充)
    + `document.body.clientWidth`混杂模式
    + `resizeTo(0,100)`
    + `resizeBy(0,100)`
        * 使用方法同moveTo/moveBy
- 导航和打开窗口
    + `window.open()`导航到一个特定的URL或者打开一个新的浏览器窗口
        * 可以接收4个参数
            - 要加载的URL
            - 窗口目标
                + 自定义的窗口名或frame名
                + `_parent`
                + `_self`
                + `_top`
                + `_blank`
            - 一个特性字符串
                + 在不打开新窗口的情况下，会忽略这个参数
                + `fullscreen`是否最大化
                + `height`新窗口高度
                + `left`新窗口左坐标
                + `location`是否在浏览器窗口中显示地址栏
                + `menubar`是否在浏览器窗口中显示菜单栏
                + `resizable`是否可以通过拖动浏览器窗口的边框改变大小
                + `scrollbars`是否允许滚动
                + `status`是否显示状态栏
                + `toolbar`是否显示工具栏
                + `top`新窗口的上坐标
                + `width`新窗口的宽度
            - 一个表示新页面是否取代浏览器历史记录当中加载页面的布尔值
        * 返回值是一个指向新窗口的引用
    + `新窗口引用.close()`关闭新打开的窗口
    + `新窗口引用.closed`检测是否关闭//true
    + `新窗口引用.opener`保存着原始窗口对象
- 间歇调用和超时调用
    + `setTimeout()`指定时间后执行代码
        * 第一个参数是要执行的代码
            - 可以是一个包含JS代码的字符串，不建议
            - 可以是一个函数
        * 第二个参数是以毫秒表示的时间
        * 返回值是一个数值ID,表示这个超时调用，这个ID是这个计划执行代码的唯一标识符，后面可通过这个标识符用`clearTimeout(timeoutId)`取消超时调用
    + `setInterval()`指定周期执行代码，直至被取消或页面被卸载
        * 参数同`setTimeout`
        * `clearInterval(intervalId)`取消周期执行代码
- 系统对话框
    + `alert()`
    + `confirm()`返回值为{OK:True,Cancel:False}
    + `prompt()`
        * 第一个参数是显示给用户的文本提示
        * 第二个参数是文本输入框的默认值
        * 返回值是{OK：文本输入框的值,Cancel：null}
    + `window.print()`弹出打印对话框
    + `window.find()`弹出查找对话框

### location对象
- 概念
    + 最有用的BOM对象之一
    + 提供了当前窗口中加载文档的有关信息，还提供了一些导航功能
    + 即使window对象的属性也是document对象的属性
        * `window.location == document.location`
    + `hash`:`#content`
    + `host`:`www.xx.com:80`
    + `hostname`:`www.xx.com`
    + `pathname`:`/demo/`
    + `port`:`8080`
    + `protocol`:`http:`
    + `search`:`?a=1&b=2`
- 查询字符串参数
    + `location.search`返回从问号到URL末尾的所有内容
    + 想逐个访问每个查询字符串的参数，可自定义函数截取字符串
- 位置操作
    + `location.assign(URL)`立即打开新URL并在浏览器的历史记录中生成一条记录
        * `window.location = URL`
        * `location.href = URL`是最常用改变浏览器位置的操作
        * 这两行代码和显式调用assign()的效果一样
    + `location.replace(URL)`会导致浏览器位置改变，但不会再历史记录中生成新纪录
    + `location.reload()`从浏览器缓存中重新加载当前显示页面
        * `location.reload(true)`强制从服务器重新加载
        * 最好将reload放在代码最后一行

### navigator对象
- 用来识别客户端浏览器的事实标准，navigator对象的属性通常用于检测显示页面的浏览器类型
- 检测插件
    + `navigator.plugins[]`
- 注册处理程序

### screen对象
- 用来表明客户端的能力
    + 浏览器窗口外部的显示器的信息

### history对象
- 保存着用户上网的历史记录,无法得知用户浏览过的URL
- `history.go()`
    + 负数表示向后跳转
    + 正数表示向前跳转
    + 字符串表示跳转到最近(前后都行)的包含这个字符串的历史记录
- `history.back()`后退一页
- `history.forward()`前进一页
- `hsitory.length`历史记录的数量

## 9.客户端检测(检测是啥浏览器)
### 能力监测
### 怪癖检测
### 用户代理检测

## 10.DOM
### 节点层次
- Node类型
- Document类型
- Element类型
- Text类型
- Comment类型
- CDATASection类型
- DocumentType类型
- DocumentFragment类型
- Attr类型

### DOM操作技术
- 动态脚本
- 动态样式
- 操作表格
- 使用NodeList

## 11.DOM拓展
### 选择符API
### 元素遍历
### HTML5
### 专有扩展

## 12.DOM2和DOM3
### DOM变化
### 样式
### 遍历
### 范围

## 13.事件
>可以使用监听器(或处理程序)来预订事件，是一种观察员模式的模型，支持页面行为和页面外观的松耦合
### 事件流
>描述从页面接收事件的顺序。IE的事件流是事件冒泡流，而网景的事件流是事件捕获流
- 事件冒泡event bubbling
  - 事件开始时由最具体的元素接收(按钮)，然后逐级向上传播到较为不具体的节点(document)
  - 所有现代浏览器都支持事件冒泡，IE9、Safari、Chrome、Firefox将事件一直冒泡到window
- 事件捕获event capturing
  - 最先由不具体的节点接收到事件，具体的元素最后收到事件
  - 目的：在事件到达目标节点之前捕获他
  - 上述浏览器也都支持这种事件流模型，从window对象开始捕获事件
- DOM事件流
  - 三个阶段：事件捕获阶段(截获)、处于目标阶段(接收)、事件冒泡阶段(响应)
  - 上述浏览器及更高版本都会在捕获阶段触发事件对象上的时间。所以捕获阶段、目标阶段都能操作事件
### 事件处理程序
>响应某个事件的函数就叫做事件处理程序或事件监听器，通常以'on'开头，区别于事件名
- HTML事件处理程序
  - 使用与事件处理程序同名的属性来指定,属性值是可以被执行的JavaScript代码，可以是外部代码
    ```html
    <input type="button" value="Click Me" onclick="showMessage()">
    ```
  - 注意
    - 存在一个局部变量event
    - this指定的是这个input元素
  - 缺点
    - 存在一个时差问题：在解析外部JavaScript代码之前就点击了按钮，会引发错误,解决方案如下
    ```html
    <input type="button" value="Click Me" onclick="try{showMessage();}catch(ex){}">
    ```
    - HTMl和JavaScript代码耦合
    - 受不同浏览器环境影响
- DOM0级事件处理程序
  - 将一个函数赋值给一个元素对象的引用的属性，属性名和事件处理程序同名
    ```javascript
    var btn = document.getElementById("myBtn");
    btn.onclick = function(){
        //
    }
    ```
  - 优势
    - 简单
    - 跨浏览器
  - 删除事件
    - `btn.onclick = null;`
- DOM2级事件处理程序
  - 定义了两种方法来处理事件：addEventListener()、removeEventListener()
  - 参数
    - 第一个参数：要处理的事件名
    - 第二个参数：作为事件处理程序的函数
    - 第三个参数：布尔值，true表示捕获阶段调用函数；false表示冒泡阶段调用函数
      - 除非想在事件到达目标之前捕获事件，不然不用true
    ```javascript
    function handler(){
        return this.id
    }
    function handler2(){
        return '2'
    }
    var btn = document.getElementById("myBtn");
    btn.addEventListener('click', handler, false)
    btn.addEventListener('cilck', handler2, false)//可以添加两个不同的click事件
    btn.removeEventListener('click', handler, false)//删除事件监听
    ```
- IE事件处理程序
  - 实现了与DOM类似的两个方法：attachEvent()、detachEvent()
  - 参数
    - 第一个参数：事件处理程序名(带'on-'的)
    - 第二个参数：事件处理程序函数
  - 和DOM事件处理程序的差异
    - this指向window，DOM指向元素引用
    - 添加两个事件时，顺序是后添加的先执行，DOM是代码顺序执行
  - 支持IE事件处理程序的有IE和Opera
- 跨浏览器的事件处理程序
  - 手写一个兼容各个浏览器的事件处理程序，三类：DOM2级、DOM0级、IE
  ```javascript
  var EventUtil = {
      addHandler:function(ele, type, fun) {
          if(ele.addEventListener){
              ele.addEventListener(type, fun, false);
          } else if (ele.attachEvent) {
              ele.attachEvent("on" + type, fun);
          } else {
              ele["on"+type] = fun;
          }
      },
      removeHandler:function(ele, type, fun){
          if(ele.removeEventListener){
              ele.removeEventListener(type, fun, false);
          }else if(ele.detachEvent){
              ele.detachEvent("on"+type, fun);
          }else{
              ele["on"+type] = null;
          }
      }
  }

  var btn = document.getElementById('myBtn');
  function handler() {
      return '1'
  };
  EventUtil.addHandler(btn, 'click', handler);
  EventUtil.removeHandler(btn, 'click', handler);
  ```
  - 现在几乎已经全部支持DOM2级事件了
### 事件对象
- DOM中的事件对象
  - 兼容DOM的浏览器会将一个event对象传入到事件处理程序中，一旦处理程序执行完成，event对象就会被销毁
- IE中的事件对象
  - DOM0级：window.event
  - attachEvent: event
- 跨浏览器的事件对象
### 事件类型
- UI事件
- 焦点事件
- 鼠标与滚轮事件
- 键盘与文本事件
- 复合事件
- 变动事件
- HTML5事件
- 设备事件
- 触摸与手势事件
### 内存和性能
- 事件委托
- 移除事件处理程序
### 模拟事件
- DOM中的事件模拟
- IE中的事件模拟

## 20.Json
### 语法
- 简单值
    + 使用与JavaScript相同的语法，可以在Json中表示字符串、数值、布尔值和null。
    + JSON不支持JavaScript中的特殊值undefined
- 对象
    + 对象作为一种复杂数据类型，表示的是一组无序的键值对儿。而每个键值对儿中的值可以是简单值，也可以是复杂数据类型的值
- 数组
    + 数组也是一种复杂数据类型，表示一组有序的值的列表，可以通过数值索引来访问其中的值。数组的值也可以是任意类型————简单值、对象或数组
    + JSON不支持变量、函数或对象实例，它就是一种表示结构化数据的格式，虽然与JavaScript中表示数据的某些语法相同，但它并不局限于JavaScript的范畴。

#### 简单值
- 数值：5
- 字符串："Hello world!"
    + JSON字符串必须使用双引号，单引号会导致语法错误
- 布尔值和null也是有效的JSON形式

#### 对象
- Javascript中的对象字面量：
    ```Javascript
            var person = {
                name: "Nicholas",
                age: 29
            };
    ```
- JSON表示上述对象的方式如下
    ```JSON
            {
                "name": "Nicholas",
                "age": 29
            }
    ```
- 与Javascript的对象字面量相比，JSON对象有两个地方不一样
    + 首先，没有声明变量(JSON中没有变量的概念)
    + 其次，没有末尾的分号

#### 数组
- JavaScript中的数组字面量
    + var values = [25,"h1",true];
- JSON中
    + [25,"h1",true]

### 解析与序列化
#### JSON对象
- 早期的JSON解析器基本上就是使用JavaScript的eval()函数。由于JSON是JavaScript语法的子集，因此eval()函数可以解析、解释并返回JavaScript对象和数组
- JSON对象有两个方法
    + stringify()和parse()
    + 在最简单的情况下，这两个方法分别用于把JavaScript对象序列化为JSON字符串和JSON字符串解析为原生JavaScript值
    ```Javascript
            var book = {
                title: "Professional JavaScript",
                authors: [
                    "Nicholas C. Zakas"
                ],
                edition: 3,
                year: 2011
            };

            var jsonText = JSON.stringify(book);
            var bookCopy = JSON.parse(jsonText);
    ```

#### 序列化选项
- JSON.stringify()除了要序列化的JavaScript对象外，还可以接收另外两个参数，这两个参数用于指定以不同的方式序列化JavaScript对象
    + 过滤器：可以是一个数组，也可以是一个函数
    + 选项：表示是否在JSON字符串中保留缩进。
- 过滤结果
    + 如果过滤器参数是数组，那么JSON.stringify()的结果中将只包含数组中列出的属性、
    ```Javascript
        var book = {
            title: "Professional JavaScript",
                authors: [
                    "Nicholas C. Zakas"
                ],
                edition: 3,
                year: 2011
        };

        var jsonText = JSON.stringify(book,["title, "edition])
    ```
    + 如果第二个参数是函数，传入的函数接收两个参数，属性名和属性值。根据属性名可以知道应该如何处理要序列化的对象中的属性。属性名只能是字符串，而在值并非键值对儿结构的值时，键名可以是空字符串。为了改变序列化对象的结果，函数返回的值就是相应键的值，不过要注意，如果函数返回了undefined，那么相应的属性会被忽略

    ```Javascript
        var book = {
            title: "Professional JavaScript",
                authors: [
                    "Nicholas C. Zakas"
                ],
                edition: 3,
                year: 2011
        };

        var jsonText = JSON.stringify(book,function(key, value){ 
             switch(key){ 
             case "authors": 
             return value.join(",") 
             case "year": 
             return 5000; 
             case "edition": 
             return undefined; 
             default: 
             return value; 
             } 
             });
    ```
- 字符串缩进
    + JSON.stringify()方法的第三个参数用于控制结果中的缩进和空白符。如果这个参数是一个数值，那它表示的是每个级别缩进的空格数
    + var jsonText = JSON.stringify(book, null, 4); 
    + 只要传入有效的控制缩进的参数值，结果字符串就会包含换行符。最大缩进空格为10，大于的会自动转换为10
- toJSON()方法
    + 原生对象有一个toJSON()方法，能够将JavaScript的date对象自动转换成ISO 8601日期字符串(与在Date对象上调用toISOString()的结果完全一样)
    ```Javascript
            var book = {
                title: "Professional JavaScript",
                authors: [
                    "Nicholas C. Zakas",
                    "sss"
                ],
                edition: 3,
                year: 2011,
                toJSON: function(){
                    return this.title;
                }
            };

            var jsonText = JSON.stringify(book);
    ```
    + toJSON()可以作为函数过滤器的补充，因此理解序列化的内部顺序十分重要
        * 如果存在toJSON()方法而且能通过它取得有效的值，则调用该方法。否则，返回对象本身。
        * 如果提供了第二个参数，应用这个函数过滤器。传入函数过滤器的值是上一步返回的值
        * 对上一步返回的每个值进行相应的序列化
        * 如果提供了第三个参数，执行相应的格式化
- 解析选项
    + JSON.parse()方法也可以接收另一个参数，该参数是一个函数，将在每个键值对儿上调用。为了区别JSON.stringify()接收的替换(过滤)函数(replacer)，这个函数被称为还原函数(reviver),但实际上这两个函数的签名是相同的————它们都接收两个参数，一个键一个值，而且都需要返回一个值。
    ```Javascript
                var book = {
                    "title": "Professional JavaScript",
                    "authors": [
                        "Nicholas C. Zakas",
                        "sss"
                    ],
                    edition: 3,
                    year: 2011,
                    releaseDate: new Date(2011,11,1)
                };

                var jsonText = JSON.stringify(book);
                
                var bookCopy = JSON.parse(jsonText, function(key,value){
                    if(key == "releaseDate"){
                        return new Date(value);
                    }else{
                        return value;
                    }
                    });

                console.log(bookCopy.releaseDate.getFullYear());
    ```

## 21.Ajax与Comet
### XMLHttpRequest对象

```javascript
function createXHR(){
    if(typeof arguments.callee.activeXString != "string"){
        var versions = ["MSXML2.XMLHttp.6.0", "MSXML2.XMLHttp.3.0",
                        "MSXML2.XMLHttp"],
                        i,len;
        for(i=0, len=version.length; i<len; i++){
            try{
                new ActiveXObject(version[i]);
                arguments.callee.activeXString = version[i];
                break;
            } catch (ex){

            }
        }
    }
    return new ActiveXObject(arguments.callee.activeXString);
}
```
- XHR的用法
  - open(),它接受3个参数
      + 要发送的请求的类型
      + 请求的URL:相对于执行代码的当前页面(也可以使用绝对路径)
      + 表示是否异步发送请求的布尔值
      + `xhr.open("get", "example.php", false)`
          * open()方法并不会真正发送请求，而只是启动一个请求以备发送。
          * 只能向同一个域中使用相同端口和协议的URL发送请求。如果URL与启动请求页面有任何差别，都会引发安全错误
      ```
      xhr.open("get", "example.txt", false);
      xhr.send(null)
      ```
  - send()，接收一个参数，
     + 即要作为请求主题发送的数据。如果不需要通过请求主题发送数据，则必须传入null，因为这个参数对有些浏览器来说是必需的。调用send()之后，请求就会被分派到服务器。
     + 收到响应后，响应的数据会自动填充XHR对象的属性，相关的属性简介如下
         * `responseText`：作为响应主体被返回的文本
         * `responseXML`：如果响应的内容类型是"text/xml"或"application/xml",这个属性中将保存着响应数据的XML DOM 文档
         * `status`：响应的HTTP状态
         * `statusText`：HTTP状态的说明

- HTTP头部信息
- GET请求
- POST请求
### XMLHttpRequest 2级
- FormData
- 超时设定
- overrideMimeType()方法
### 进度事件
- load事件
- progress事件
### 跨域资源共享
- IE对CORS的实现
- 其他浏览器对CORS的实现
- Preflighted Requests
- 带凭据的请求
- 跨浏览器的CORS
### 其他跨域技术
- 图像Ping
- JSONP
- Comet
- 服务器发送事件
- Web Sockets
- SSE与Web Sockets
### 安全

## 22.高级技巧
### 高级函数
### 防篡改对象
### 高级定时器
### 自定义事件
### 拖放

## 23.离线应用与客户端存储
### 离线监测
### 应用缓存
### 数据存储
- Cookie
- IE用户数据
- Web存储机制
- IndexedDB
## 24.最佳实践
### 可维护性
### 性能
### 部署

# ES6
## 11.Promise与异步编程
### 异步编程
- 什么是异步编程
  - JavaScript引擎是基于单线程事件循环概念构建的
  - 任务队列：JavaScript引擎同一时刻只能执行一个代码块，所以需要跟踪即将运行的代码，所以任务队列就是用来存储这些即将运行的代码，让他们排成一个队列，每当一段代码准备执行时，都会被添加到任务队列中，
  - 事件循环：负责监控代码执行并管理任务队列
  - [JavaScript 异步、栈、事件循环、任务队列](https://segmentfault.com/a/1190000011198232)
- 事件模型
  - 见JavaScript高级程序设计中介绍的 [事件](#13.事件)
  - 事件模型适用于处理简单的交互，因为无法总是保证事件处理程序在事件触发之前已经加载完成( 即用户可能在onclick函数没加载完成之前就已经在疯狂点击button了)
- 回调模式
  - 回调模式中被调用的函数作为参数传入
  - 问题：回调地狱难以理解和调试
### Promise基础
- 什么是Promise
  - 相当于异步操作结果的占位符，它不去订阅事件，也不传递一个回调函数，而是让函数返回一个Promise
    ```javascript
    var promise = readFile("helloworld.txt")
    //代码开始时，readFile()不会立即开始读取文件，首先会返回一个Promise对象表示异步读取操作
    //未来如何操作这个对象取决于Promise的生命周期
    ```
- Promise的生命周期
  - 生命周期
    - 两个状态：未处理和已处理；三个状态：进行中、成功、失败
      - unsettled   未处理
        - pending   进行中
      - settled     已处理
        - fulfilled 成功
        - rejected  失败
  - [[PromiseState]]内部属性来表示Promise的三个状态，无法访问
  - then()方法
    - Promise对象通过then()方法来根据特定状态执行特定操作
    - 参数
      - 第一个参数是当promise状态为fulfilled时调用的函数
      - 第二个参数是当promise状态为rejected时调用的函数
      - 两个参数都是可选的
    - thenable对象
      - 一个对象实现了then方法，就可以称之为thenable对象
      - 所有Promise对象都是thenable对象，反之不然
  - catch()方法
    - 和只传入拒绝处理程序的then()方法等价  
        ```javascript
        promise.catch(function(err){
            console.error(err.message)
        })
        //等价于
        promise.then(null, function(err){
            console.error(err.message)
        })
        ```
  - 每次调用then()方法或catch()方法都会创建一个新任务，当promise被解决时执行，这些任务会被加入到一个为promise量身定制的独立任务队列
- 创建未完成的Promise
  - 用Promise构造函数创建Promise
    - 构造函数只接受一个参数：包含初始化Promise代码的执行器(executor)函数
    - 执行器函数接受两个参数：resolve函数(执行器成功时调用)和reject函数(执行器失败时调用)
     ```javascript
    let fs = require('fs');
    function readFile(filename) {
        let exec = function(resolve, reject) {
            //触发异步操作
            fs.readFile(filename, { encoding: "utf-8" }, function(err, contents) {
                //检查是否有错误
                if (err) {
                    reject(err)
                    return
                }
                //成功读取文件
                resolve(contents)
            })
        }
        return new Promise(exec)
    }

    let promise = readFile("example.txt")
    
    promise.then(function(contents) {
        console.log(contents)
    }, function(err) {
        console.error(err.message)
    })
     ```
    - Promise的执行器会立即执行,无论是调用了resolve还是reject，都会将一个新任务推入任务队列
    ```javascript
    let promise = new Promise(function(resolve, reject) {
      console.log('promise')
    })
    console.log('window')
    //promise
    //window
    setTimeOut(function() {
        //也将新任务推入了任务队列，只不过要求这个任务在500ms后执行，所以比window后显示
        console.log('setTimtout')
    }, 500)
    console.log('window')
    //window
    //setTimeout
    ```
    - 执行函数调用resolve()或reject()后，会触发一个异步操作，传入then方法的函数此时会被添加到任务队列中，并异步执行(可以理解成resolve()是一个发射器，promise.then()的第一个参数的函数是这个发射器的接收装置，这个函数的参数就是发射器传过来的参数)
    ```javascript
    let promise = new Promise(function(resolve, reject) {
        console.log('promise')
        resolve('resolve')
    })
    promise.then(function(c) {
        //完成处理程序和拒绝处理程序总是在执行器完成后再被添加到任务队列的末尾
        console.log(c)
    })
    console.log('window')
    //promise
    //window
    //resolve

    ```

- 创建已处理的Promise
  - 为什么要创建已处理的Promise
    - 如果你还不知道给用Promise来表示什么值的时候，可以用new创建一个未处理的Promise
    - 如果你知道要用Promise来表示什么值的时候，再大张旗鼓的new一个Promise，在Promise中加入执行器函数有点多余，所以这时候需要创建处于settled状态的Promise
  - Promise.resolve()
    - 只接受一个参数并返回一个完成状态的Promise
    ```javascript
    let promise = Promise.resolve(42)
    promise.then(function(content) {
        console.log(content) //42
    })
    ```
  - Promise.reject()
    - 只接受一个参数并返回已拒绝状态的Promise
    ```javascript
    let promise = Promise.reject(42)
    promise.then(null, function(err) {
        console.log(err) //42
    })

    promise.catch(function(err) {
        console.log(err) //42
    })
    ```
    - 如果向Promise.resove()或Promise.reject()传入一个Promise对象，会直接返回这个对象，可以用此方法来判断一个对象是不是Promise对象
    - 如果向Promise.resolve()或Promise.reject()传入一个非Promise对象的Thenable对象，会创建一个新的Promise对象(Promise.resolve:pending状态;Promise.reject:rejected状态)，并在then函数中被调用
  - 非Promise的Thenable对象
    - 拥有一个接受resolve和reject这两个参数的方法并且这个方法名叫then方法的普通对象就是非Promise的Thenable对象
    ```javascript
    //1.使用Promise.resolve创建基于Thenable的已完成Promise
    let thenable = {
        then:function(resolve, reject) {
            resolve(42)
        }
    }
    //Promise.resolve调用的是thenable.then()，返回的是一个pending状态Promise
    let p1 = Promise.resolve(thenable)
    p1.then(function(c) {
        //此时p1是一个pending状态Promise对象
        console.log(c) //42
    })
    
    //2.使用Promise.resolve创建基于Thenable的已拒绝Promise
    let thenable = {
        then:function(resolve, reject) {
            reject(42)
        }
    }
    //Promise.resolve调用的是thenable.then()，返回的是一个pending状态Promise
    let p1 = Promise.resolve(thenable)
    p1.catch(function(c) {
        console.log(c) //42
    })

    //3.使用Promise.reject创建基于Thenable的已拒绝Promise
    let thenable = {
        then:function(resolve, reject) {
            reject(42)
        }
    }
    //Promise.reject会返回一个已拒绝状态的Promise对象
    let p1 = Promise.reject(thenable)
    p1.catch(function(c) {
        console.log(c) //thenable对象
    })

    //4.使用Promise.reject创建基于Thenable的已完成Promise
    let thenable = {
        then:function(resolve, reject) {
            resolve(42)
        }
    }
    //Promise.reject会返回一个已拒绝状态的Promise对象
    let p1 = Promise.reject(thenable)
    p1.then(function(c) {
        //由于p1此时已经是一个已拒绝状态的Promise对象
        console.log(c) //UnHandlePromiseRejectionWarning
    })
    ```
- 执行器错误
  - 如果执行器内部抛出错误，则Promise的拒绝处理程序就会自动被调用
    ```javascript
    let promise = new Promise(function(resolve, reject) {
        throw new Error('I am a Problem')
    })
    promise.catch(function(err) {
        console.log(err.message) //I am a Problem
    })


    //原因是每个执行器中都隐藏了一个try-catch语句

    let promise = new Promise(function(resolve, reject) {
        try {
            throw new Error('error')
        } catch(ex) {
            reject(ex)
        }
    })
    ```

### 全局的Promise拒绝处理
>如果在没有catch或then的拒绝处理程序的情况下拒绝一个Promise，不会提示失败信息
```javascript
let rejected = Promise.reject(42)
// rejected此时还没有被处理，rejected此时是一个rejected状态的Promise对象
//但是会报UnHandlePromiseRejectionWarning
rejected.catch(function(err) {
    //此时rejected已经被处理
    console.log(err) //42
})
```
>明明已经被Promise.reject()立即拒绝的Promise(按理来说已拒绝就是处理了)，可是我们知道要等到catch来处理才能真正算上Promise已处理(就很生硬，明明已经明文reject了)，但在不用catch/then之前却很难知道已拒绝的Promise何时被处理，所以引入全局拒绝处理
- Node.js环境下
  - 触发process对象上的两个事件：unhandledRejection和rejectionHandled
  - 触发条件是：当Promise被拒绝，且没有拒绝处理程序(catch/then)时
  - 目的：是为了识别那些已经被拒绝却还没被处理过的Promise
  - unhandledRejection事件处理程序
    - 接受两个参数，第一个参数是拒绝原因(错误对象)，第二个参数是已拒绝的Promise
    ```javascript
    let rejected
    //监听unhandledRejection事件
    process.on('unhandledRejection', function(reason, promise) {
        console.log(reason.message == 'error') //true
        console.log(promise == rejected) //true
    })
    rejected = Promise.reject(new Error('error'))
    ```
  - rejectionhandled事件处理程序
    - 接受一个参数，已拒绝的Promise对象
    - 触发：在拒绝处理程序最后被调用时触发(异步控制最后调用)，但在同步状态(即已拒绝的Promise和catch()在一个事件循环中)有拒绝处理程序时会被忽略。
    ```javascript
    let rejected = Promise.rejecte(new Error('error'))

    process.on('rejectionHandled', function(promise) {
        console.log(promise == rejected)  
    })

    setTimeout(function(){
        rejected.catch(function(err) {
            console.log(err.message) 
        })
    }, 1000)

    //error
    //true ，如果catch调用不在延时函数里，则不会触发rejectionHandled事件
    ```
  - 实现一个Node.js环境下简单的未处理拒绝跟踪器
    ```javascript
    let possiblyUnhandledRejections = new Map()
    process.on('unhandledRejected', function(reason, promise) {
        possiblyUnhandledRejections.set(promise, reason)
    })

    process.on('rejectionHandled', function(promise) {
        possiblyUnhandledRejections.delete(promise)
    })

    setInterval(function() {

        possiblyUnhandledRejections.forEach(function(reason, promise) {
            console.log(reason.message ? reason.message : reason)
            //做一些什么来处理这些拒绝
            handleRejection(reason, promise)
        })

        possiblyUnhandledRejections.clean()
    }, 60000)
    ```

- 浏览器环境下
  - 通过触发两个在window对象上的事件来识别未处理的拒绝
  - unhandledrejection和rejectionhandled:触发条件和Node.js环境下相同
    - 值得注意的是，浏览器下的事件名和事件的差异，即事件名是不带'on'的，但window调用的事件处理程序即事件监听器是要带'on'的
  - 与Node.js环境下差异
    - 参数差异
      - Node.js下是接受多个独立参数(reason, promise)
      - 浏览器下是接受一个event对象，这个对象有以下属性
        - type：事件名称(unhandledrejection或rejectionhandled)
        - promise：被拒绝的promise对象
        - reason：来自被拒绝的promise对象的拒绝值(即Promise.reject()或者执行器中的reject()括号中的拒绝值)
    - 浏览器的两个事件都可以使用reason，而Node.js下handledRejection事件不能使用
        ```javascript
        let rejected
        window.onunhandledrejection = function(event) {
            console.log(event.type) //unhandledrejection
            console.log(event.reason.message) //error
            console.log(event.promise === rejected) //true
        }

        window.onrejectionhandled = function(event) {
            console.log(event.type) //rejectionhandled
            console.log(event.reason.message) //error
            console.log(event.promise === rejected) true
        }
        rejected = Promise.reject(new Error('error'))
        ```
    - 实现一个简单的未处理拒绝跟踪器
    ```javascript
    let possiblyUnhandledRejections = new Map()
    window.addEventListener('unhandledRejected', function(event) {
        possiblyUnhandledRejections.set(event.promise, event.reason)
    },false)

    window.addEventListener('rejectionHandled', function(event) {
        possiblyUnhandledRejections.delete(event.promise)
    })

    setInterval(function() {

        possiblyUnhandledRejections.forEach(function(reason, promise) {
            console.log(reason.message ? reason.message : reason)
            //做一些什么来处理这些拒绝
            handleRejection(reason, promise)
        })

        possiblyUnhandledRejections.clean()
    }, 60000)
    ```
### 串联Promise
- 为什么能串联
  - 因为每次调用then或catch时返回一个新的Promise，只有当第一个Promise被处理后，第二个甚至更多才会被处理
    ```javascript
    let p1 = new Promise(function(resolve, reject) {
        resolve(42)
    })

    p1.then(function(content) {
        console.log(content)
    }).then(function() {
        console.log('then2')
    })

    //42
    //then2
    ```
- 捕获错误
  - 务必在Promise链的末尾留一个拒绝处理程序以确保能够正确处理所有可能发生的错误
- Promise链的返回值
  - Promise链的一个重要特性就是可以使用return给下游的Promise传递数据
- 在Promise链中返回Promise
  - 可以将Promise对象return给下一个处理程序，这个Promise对象可以在全局定义，也可以在当前处理程序内部定义
### 响应多个Promise
- Promise.all()
  - 接受一个参数，返回一个Promise
  - 参数是一个含有多个受监控的Promise的可迭代对象(例如，一个数组)，只有当这个可迭代对象中所有的Promise对象被处理后，返回的Promise才会被处理，只有当所有的Promise对象resolved后，然后的Promise才会resolved，并且resolved的结果会按相同的迭代方式返回；rejected就直接返回reject()的那一个，后面的就不管了了
- Promise.race()
  - 顾名思义race就是竞赛，接受的参数和返回值和all()方法一模一样，但是只要有一个符合要求就直接返回，不会像all()一样，resolved就要等所有的resolved，返回一个resolved的可迭代方式，race()是只要谁第一个resolved的就返回这个，rejected也同理
### 自Promise继承
- Promise与其他内建类型一样，可以作为基类派生出其他类，所以可以自定义扩展内建Promise的功能
### 基于Promise的异步任务执行
- 返回去学习第九章生成器
 
# 你不知道的JS
## 作用域和闭包
### 作用域是什么 
- 作用域是一套设计良好的规则。用来存储变量，并且之后可以方便的找到这些变量。

#### 编译原理
- 传统编译语言的流程中，程序中的一段源代码在执行之前会经历三个步骤
    + 分词/词法分析(tokenizing/lexing)
        * 词法化(单词化)这个过程会将字符组成的代码分解成有意义的代码块(词法单元)
        * `var a = 1;`被分解成var、a、=、1、;。空格在关键的地方会被当做词法单元
        * 词法分析是*有状态*的解析规则进行的(即`ab`分成`a`和`b`还是`ab`要判断语境)
    + 解析/语法分析(Parsing)
        * 这个过程将词法单元流(数组)转换成一个代表了程序语法结构的由元素逐级嵌套所组成的的树(抽象语法树,AST)。
        * `var a = 1;`转换成的抽象语法树有一个叫VariableDeclaration(变量声明)的顶级节点，接下来是一个值为a叫做Identifier(标识符)的子节点，以及一个值为=叫做AssignmentExpression(赋值表达式)的子节点。AssignmentExpression有一个值为1叫做NumericLiteral(数字文字)的子节点
    + 代码生成
        * 这个过程将AST转换为可执行代码。这个过程和语言、目标平台息息相关
        * 将`var a = 1;`的AST转化为一组机器指令，用来创建一个叫做a的变量(包括分配内存等)，并将一个值存储在a中
- JavaScript代码片段不是提前编译的，它 **就在** 执行前进行编译，编译发生在代码执行前几微秒甚至更短。编译结果不能在分布式系统中进行移植
    + JavaScript编译器会对`var a = 1;`进行编译，然后做好执行它的准备，并通常马上执行

#### 理解作用域
- 引擎
    + 职责：从头到尾负责整个JavaScript程序的编译及执行过程
    + 术语：LHS和RHS
        + 在使用变量时，引擎会通过这两种查找来判断变量是否被声明
        + 分别表示赋值操作的左侧和右侧
        + LHS：目的是对变量进行赋值，对哪个变量赋值就对哪个变量进行LHS引用。对变量显式的赋值或者调用函数时传入实参就是LHS引用,如a = 1
        + RHS：目的是获取变量的值，获取哪个变量的值就是对哪个变量进行RHS引用。通过引用变量来获取值就是RHS引用，如console.log(a)
       
- 编译器
    + 职责：引擎的好朋友，负责词法分析、语法分析及代码生成等脏活累活
    + 变量的赋值操作：会执行两个动作
        + 首先编译器会在当前作用域中声明一个变量(如果之前没声明过)。这会在最开始的阶段，代码执行前进行。
        + 然后在运行时引擎会在作用域中查找该变量，如果能够找到就会对它赋值
- 作用域
    + 职责：引擎的另一位好朋友，负责收集并维护所有变量(声明的标识符)组成的一系列查询，并实施一套非常严格的规则，确定当前执行的代码对这些标识符的访问权限。

#### 作用域嵌套
- 在当前作用域种无法找到某个变量，引擎就会在外层嵌套的作用域种继续查找，直到找到该变量为止。
- 作用域链

#### 异常
- 为什么要区分LHS和RHS
    + 因为在变量没有被声明的情况下这两种查询的行为是不一样的
    + 用RHS引用查看变量是否被声明时，如果没声明(整条作用域链中)则抛出异常ReferenceError(引用异常，同作用域判别失败相关)
    + 用LHS引用查看变量是否被声明时，非严格模式下不会抛出异常，而且全局作用域中会创建该变量，并将其返还给引擎。严格模式下会抛出跟RHS一样的异常
    + 若RHS找到了变量，但尝试对这个变量做不合理的操作，如null.getName()会抛出异常TypeError(类型异常，作用域判别成功，对判别结果的操作异常)

### 词法作用域
- 作用域共有两种主要的工作模型
    + 词法作用域
    + 动态作用域

#### 词法阶段
- 词法作用域就是定义在词法阶段的作用域。
- 词法作用域是由你在写代码时将变量和块作用域写在哪来决定的，因此当词法分析器处理代码时会保持作用域不变(除非使用欺骗词法作用域的方法)
- 查找：作用域会在找到第一个匹配的标识符停止
- 无论函数在哪里被调用，也无论它如何被调用，它的词法作用域都只由函数被声明时所处的位置决定。

#### 欺骗词法
- 欺骗词法作用域会导致性能下降
- `eval`和`with`能实现欺骗词法的目的
    + `eval()`接受一个字符串作为参数，并将其内容视为好像在书写代就存在于这个位置的代码。eval中的声明可以在运行期修改书写期的词法作用域
        + 严格模式下，eval中的声明无法修改所在的作用域
        + `setInterval`和`setTimeout`的第一个参数也可以是字符串类似于eval。不提倡
        + `new Function`的最后一个参数也可以接受字符串，避免使用
    - `with` 通常被当做重复引用同一个对象的多个属性的快捷方式，可以不需要重复引用对象本身
        + with可以将一个没有或有多个属性的对象处理为一个完全隔离的词法作用域
        + 尽管with块可以将一个对象处理为词法作用域，但是这个块内部正常的var声明并不会被限制在这个块的作用域，而是被添加到with所处的作用域中
- eval函数如果接受了含有一个或多个声明的代码的字符串，就会[修改]其所处的词法作用域
- with声明实际上是根据你传递给它的对象凭空 [创建了一个全新] 的词法作用域
- 一个不推荐使用eval和with的原因是会被严格模式所影响

#### 性能
- 引擎会在编译阶段进行数项的性能优化。其中有些优化依赖于能够根据代码的词法进行静态分析，并预先确定所有变量和函数的定义位置，才能在执行过程中快速找到标识符

### 函数作用域和块作用域
#### 函数中的作用域
- 属于这个函数的全部变量都可以在整个函数的范围内使用及复用

#### 隐藏内部实现
- 规避冲突
    + 全局命名空间
    + 模块管理

#### 函数作用域
- 匿名和具名
- 立即执行函数表达式

#### 块作用域
- with
- try/catch
    + catch语句
- let
- const

### 提升
#### 变量声明提升和函数声明提升
- 提升：变量和函数声明从它们在代码中出现的位置被移动到作用域最顶端的过程
- 只有声明本身会被提升，而赋值或其他运行逻辑会留在原地

#### 编译器处理提升
- 包括变量和函数在内的所有声明都会在任何代码被执行前首先被处理
- 函数表达式不会提升，若在函数表达式初始化函数之前调用函数会报TypeError
```JavaScript
foo();//TypeError，此时foo不是函数，是undefined
bar();//ReferenceError
var foo = function bar (){
    ...
}
```

#### 函数优先
- 函数声明提升优先于变量声明提升

### 作用域闭包
- 当函数可以记住并访问所在的词法作用域时，即使函数是在当前词法作用域之外执行。就产生的闭包

#### 实质问题
- 闭包定义：当函数在其本身的词法作用域以外执行时，闭包就产生了
- 词法作用域的查找规则只是闭包的一部分，也是非常重要的一部分
- 几个关于闭包的说法：
    + 闭包是一个函数
    + 闭包一个作用域的容器
    + 闭包是一个引用，内部函数对外部作用域的引用
    + 闭包是一个标准，关于如何在函数作为值按需传递的词法环境中书写代码的标准
    + 总结：闭包让函数在别处被调用时可以继续访问定义时的词法作用域
- 内部函数具有一个涵盖包含函数作用域的闭包
- 无论通过何种手段将内部函数传递到所在的此法作用于以外，它都会持有对原始定义作用域的引用，无论在何处执行这个函数都会使用闭包
- 自执行函数没用闭包，但同闭包息息相关
    + 息息相关：IIFE是最常用来创建被封闭起来的闭包的工具
    + 没用到闭包：函数并不是在其本身的词法作用域以外执行
- 只要用了回调函数就在使用闭包

#### 循环和闭包
```JavaScript
for(var i = 1; i <= 5; i ++){
    setTimeout(function(){
            console.log(i)
        },i * 1000);
}
//每秒一次共输出5个6
```
- 原因：i是全局作用域中声明，延迟函数的回调会在循环结束时执行。循环结束时i=6
- 解决方案：
    + IIFE内部换一个迭代参数
    + let i=1

#### 模块
- 模块机制
    + 模块是利用闭包的代码模式中最强大的一个
    + 最常见的实现模块模式的方法通常被称为 **模块暴露**
    + 模块模式的两个必要条件
        * 必须有外部的封闭函数(引入包装函数)，该函数必须至少被调用一次，每次调用都会创建一个新的模块实例
        * 封闭函数必须返回至少一个内部函数，这样内部函数才能在私有作用域中形成闭包，并且可以访问或者修改私有的状态
    + 一个从函数调用所返回的只有数据属性而没有闭包函数的对象并不是真正的模块
        * 说明：函数调用的返回值中没有闭包函数的对象不是模块
- 现代的模块机制
    + 基于函数的模块
    + 大多数模块依赖加载器/管理器。本质上都是将这种模块定义封装进一个友好的API
    ```JavaScript
    //封装进一个友好的API
    var myModules = (function(){
        var modules = {};
        
        var get = function(name){
            return modules[name]
        }
    
        
        var define = function(name,deps,impl){
            
            for(var i=0; i<deps.length; i++){
                deps[i] = modules[deps[i]]
            }
            modules[name] = impl.apply(impl,deps)
        }


        return {
            get:get,
            define:define
        }
        })()

    //使用友好的API定义模块
    myModules.define("bar",[],function(){
        function hello(who){
            return "hello" + who;
        }
        return {
            hello:hello
        }
        })

    myModules.define("foo",["bar"],function(bar){
        var hungry = "hippo";
        function awesome(){
            console.log(bar.hello(hungry).toUpperCase());
        }

        return {
            awesome: awesome
        }
        });

    var bar = myModules.get("bar");
    var foo = myModules.get("foo");

    console.log(bar.hello("hippo"))
    foo.awesome()
    ```

- 未来的模块机制
    + ES6中为模块增加了一级语法支持
        通过模块系统进行加载时，ES6会将文件当做独立的模块来处理。每个模块都可以导入其他模块或特定的API成员，同样也可以导出自己的API成员
    + ES6模块相比基于函数的模块更加稳定
        * 基于函数的模块无法被编译器识别，API语义只有在运行时才会被考虑。因此可以在运行时修改一个模块的API
        * ES6模块的API不会在运行时改变，编译器会在编译期间对导入模块API成员的引用检查是否真实存在，若不存在会在运行时更早的抛错
    + ES6模块必须被定义在独立的文件中，即一个文件一个模块。浏览器或引擎可以在导入模块时异步的加载模块文件
    ```JavaScript
    bar.js
        function hello(who){
            return "hello" + who;

        }
        export hello;

    foo.js
        //导入bar模块中的hello函数
        import hello from "bar"
        var hungry = "hippo";
        function awesome(){
            console.log(hello(hungry).toUpperCase())
        }

        export awesome;

    baz.js
        //导入完整的模块
        module foo form "foo";
        module bar form "bar";

        console.log(bar.hello("lzm"))
        bar.awesome()
    ```
    + import 将一个模块中的一个或多个API导入到当前作用于中，并分别绑定在一个变量上
    + module 将整个模块的API导入并绑定到一个变量上
    + export 将当前模块的一个标识符导出为公共API

### 附录
#### 动态作用域
- JavaScript不具有动态作用域
- 动态作用域与this机制
- 动态作用域的作用域链是基于调用栈的，而不是代码中的作用域嵌套
- 区别
    + 词法作用域是在定义时确定的，关注函数在何处声明
    + 动态作用域是在运行时确定改的，关注函数从何调用

#### 块级作用域的替代方案
```JavaScript
{
    let a = 2;
    console.log(a)//2
}
console.log(a)//ReferenceError
```
- ES6之前实现：ES3 catch
```JavaScript
try{
    throw 2
}catch(a){
    console.log(a)//2
}
console.log(a)//ReferenceError
```
- Traceur
    + google维护的项目，该项目将ES6代码转换成兼容ES6之前的环境
    ```JavaScript
    //Traceur将ES6块作用域的代码片段转换成下列代码
    {
        try {
            throw undefined
        } catch(a){
            a = 2
            console.log(a)
        }
    }
    console.log(a)
    ```
- 隐式和显式作用域
    + let关键字隐式的创建块作用域
    + let声明会创建一个显式的作用域并进行绑定(需要使用工具let-er)
    ```JavaScript
    //let 声明,使用let-er工具
    let(a=2){
        console.log(a)
    }
    ```
- 性能
    + try/catch的性能很糟糕，但正在改进
    + IIFE不是一个普适性的方案，因为它毕竟是一个函数

#### this词法
- 箭头函数
```JavaScript
var foo = a =>{
    console.log(a)
}
foo(2) //2
```
- 箭头函数引入了叫this词法的行为
    + 箭头函数涉及this绑定的行为和普通函数this绑定的行为不一致
    + 箭头函数用当前的词法作用域覆盖了this的本来的值，而不是运行时作用域
    + 箭头函数继承外层函数调用的this绑定
- 箭头函数不理想
    + 混淆使用两种this
    + 匿名函数不具有可读性
- 用bind()代替箭头函数
- 箭头函数不仅仅意味着少写代码

## this和对象原型
### 关于this
#### 为什么要用this
- this提供一种更优雅的方式来隐式传递一个对象引用，使得代码更加简洁和易于复用

#### 误解
- this指向自身
- this指向函数作用域
    + this在任何情况下都不指向函数的词法作用域

#### this到底是什么
- this的绑定和函数声明的位置没有关系，只取决于函数的调用方式
- this是函数调用时活动对象的一个属性，arguments和函数参数也是活动对象的属性

### this全面解析
#### 调用位置
- 调用位置：函数被调用的位置。调用位置就在当前执行函数体内的前一个调用中。
- 调用栈：存放了为了到达当前执行位置所调用的所有函数。

#### 绑定规则
- 默认绑定
    + 独立函数调用，指向全局
    + **函数体内**(而不是调用位置)在严格模式下绑定到undefined，否则绑定到全局变量
- 隐式绑定
    + 函数作为对象的方法，指向对象
    + 隐式丢失
        * 把对象方法赋值给另一个变量。`var foo = obj.bar`
        * 将对象方法作为参数传入回调函数，传递参数是一种隐式赋值。`doBar(obj.bar)`
- 显式绑定-因为可以直接指定this的绑定对象
    + call()和apply()
    + 硬绑定
        * 创建一个包裹函数
        * 创建一个可以重复使用的辅助函数
        * ES5 Function.prototype.bind(this)
            - 返回一个硬编码的新函数它会把参数设置为this的上下文并调用原始函数
            ```JavaScript
            function bind(fn,obj){
                return function(){
                    return fn.apply(obj,arguments)
                }
            }
            ```
    + API调用的上下文
        * forEach的第二个可选参数，实际上是通过call/apply实现显式绑定
- new绑定
    + 使用new来调用函数，即发生构造函数调用
        * 创建一个全新的对象`new Object()`
        * 将构造函数的作用域赋给新对象(为了this指向新对象)
        * 执行构造函数中的代码(为这个新对象添加属性)
        * 如果函数没有return，那么new函数调用会返回这个新对象

#### 优先级
- new > 显示 > 隐式 > 默认
- 判断this
    + 函数是否在new中被调用?如果是，this绑定的是新创建的对象
    + 函数是否通过call/apply/bind调用？如果是，this绑定的是指定对象
    + 函数是否在某个上下文对象中被调用？如果是，this绑定的是上下文对象
        * `obj.foo()`obj的作用域即是foo函数的上下文
        * `var bar = obj.foo()`声明bar的作用域即是foo函数的上下文
    + 如果都不是，使用默认绑定。严格模式下，绑定到undefined，否则绑定到全局变量

#### 绑定例外
- 被忽略的this
    + 使用null、undefined作为this绑定对象传入call、apply、bind
        * 使用foo.apply(null,array)展开数组,foo函数定义展开的方式
            - ES6新增...操作符可以代替展开数组
        * 使用bind(null,arguments..)预设一些参数实现柯里化
        * 副作用：可能修改全局对象
    + 更安全的this
        * 传入一个特殊的对象DMZ(demilitarized zone非军事区)，而不是传入null
        * var DMZ = Object.create(null)
        * create比{}创建的对象更空，因为不创建prototype
- 间接引用
    + (b=a)的意思是将a赋值给b并返回b，属于LHS,若不存在b会创建b
    + 默认绑定
- 软绑定
    + 硬绑定会大大降低函数灵活性，无法再修改this
    + 实现：给默认绑定指定一个全局对象和undefined以外的值

#### 重提this词法
- 箭头函数不适用this的四种标准规则，而是根据外层作用域来决定this
- 箭头函数最常用回调函数，比如时间处理器或者定时器
- ES6之前在外层作用域中`var that = this`保留外层作用域中的this
- 只使用词法作用域并完全抛弃错误this风格的代码
    + 错误this风格指的是使用`var that = this`或者箭头函数，
    + 完全使用this机制和bind()

### 对象
#### 对象语法
- 两种定义对象形式
    + 对象字面量`var myObj = { key: value }`
    + 构造形式`var myObj = new Object()`

#### 对象类型
- 数据类型
    + string
    + number
    + boolean
    + null
        * 本身是基本类型，但typeof null //object
    + undefined
    + object
        * function
        * array
- 内置对象
    + String
    + Number
    + Boolean
    + Object
    + Function
    + Array
    + RegEx
    + Error
    + Date

#### 对象的内容
- 属性：对象的内容是由一些存储在特定命名位置的值组成的，称之为属性
    + 访问值两种方法
        * `.`属性访问
        * `[]`键访问
        * 区别：
            - 键访问可以用字符串计算确定属性名`['l'+'zm']`,使用非字符串会转成字符串
            - 属性访问要求属性名满足标识符命名规范；键访问可以接受任意字符串
- 可计算属性名
    + ES6增加了可计算属性名`{[ pro + "bar"]: "hello"}`
    + ES6符号Symbol：一个不透明且无法预测的值`{[Symbol.sth] = "hello"]}`
- 属性与方法
    + 方法：对象的函数
    + 函数永远不会只成为一个对象的属性，函数和对象的关系最多也只是间接关系
    + 最保险的说法，函数和方法再JavaScript中可以互换
    + ES6新增super引用，class中有时候把super绑定的函数称为方法，语义上的差别。但本质上也是间接关系。因为函数不会属于对象，只是对于相同函数对象的多个引用
- 数组
    + 数组是一套更加结构化的值存储机制，不过不限制值的类型
    + 数组也是对象，可以给数组添加属性`array.pro = value //["pro":"value"]`但length不会加长。但是不建议使用数组当做键值对对象使用
    + 如果添加的属性名可以转成数字，那么会被当做下标`array["4"] = value //[empty,empty,empty,empty,value]`
- 复制对象
    + 浅复制
        * 新对象复制旧对象的值，新对象内部的属性和旧对象内部的属性的引用对象相同，即修改旧对象，新对象也会修改，因为引用的是同一个地址的对象
        * ES6 Object.assign()
    + 深复制
        * 新对象复制旧对象之外还复制旧对象的属性
        * 实现
            - 递归浅复制，把旧对象的属性遍历复制给新对象
            - 对于JSON安全的对象，即可以被序列化且可以解析的对象
                `var newObj = JSON.parse(JSON.stringify(obj))`
- 属性描述符
    + 
- 不变性
    + 对象常量
        * writable：false
        * configurable：false
    + 禁止扩展
        * Object.preventExtensions(Obj)禁止一个对象添加新属性并保留已有属性
        `Object.PreventExtensions(obj); obj.b = 3; obj.b//undefined`
    + 密封
        * Object.seal()创建一个密封的对象
        * 实现：在现有对象上调用preventExtensions()并把所有属性configurable:false
        * 密封之后不能修改添加新属性，也不能重新配置或delete任何属性，可以修改值
    + 冻结
        * Object.freeze()创建一个冻结对象
        * 实现：在现有对象上调用seal()并把所有属性标记为writable:false
        * 冻结之后，无法修改值
        * 冻结拥有最高级别的不变性
    + 上述所有方法创建的都是浅不变性，即只会影响目标对象和其直接属性，若目标对象引用其他对象，其他对象的内部不受影响，仍然可变。若需要深不变性，遍历引用的所有的对象并调用相应方法即可。很少需要深不变性
- `[[Get]]`
    + 对象的属性访问实际上是实现了[[Get]]操作
    + 如果当前对象和原型链都没有找到相同名称的属性，会返回undefined
- `[[Put]]`
    + 设置属性或创建属性
- Getter和Setter
    + 都是隐藏函数，分别在获取属性值时和设置属性值时调用
    + 当同时给属性定义getter和setter时，此属性会被定义为访问描述符，它们的value和writable特性会被忽略
    + 两种方法配置
        * 对象字面量中`get a(){}`
        * Object.defineProperty(obj,prop,{get:f,set:f})
        ```JavaScript
        var obj = {
            get a(){
                return 1
            }
        }

        Object.defineProperty(obj,'b',{
            get:function(){
                return 2
            }
            })
        ```

- 存在性
    + `prop in obj`检查属性是否在对象及其原型链中
        * `in`检查属性名是否存在而不是值，不能用来检查值在不在数组中
    + `obj.hasOwnProperty(prop)`检查属性是否在对象中
    + `Object.prototype.hasOwnProperty.call(obj,prop)`判断存在性的强硬方法
    + 可枚举
        * 可以出现在对象属性的遍历中`enumerable:true`
        * `for in`最好只应用在对象上
        * `obj.propertyIsEnumberable(prop)`检查给定的属性名是否直接存在于对象中并满足enumerable:true
        * `Object.keys(obj)`返回一个数组，包含所有可枚举属性
        * `Object.getOwnPropertyNames(obj)`返回一个数组，包含所有属性

#### 遍历
- 遍历属性
    + 遍历对象
        * `for in`
    + 遍历数组
        * `for`遍历数组下标指向值
        * ES5数组的辅助迭代器 `forEach` `every` `some`
            - forEach忽略回调函数的返回值
            - every一直运行到回调函数返回值为false
            - some一直运行到回调函数返回值为true
            - every和some类似于for循环中的break
- 直接遍历值
    + ES6 `for of`
        * 被访问对象请求一个迭代器对象，通过调用迭代器对象的next方法遍历所有返回值
        * 数组有内置的@@iterator，对象需要定义迭代器
        * @@iterator本身不是一个迭代器对象，而是一个返回迭代器对象的函数，使用时需要函数执行`myArr[Symbol.iterator]()`
        * `next()`返回形式`{value:.., done:..}`done表示遍历是否结束
        * 每次调用迭代器对象的next()内部指针都会向前移动并返回对象属性列表的下一个值
    + 使用
    ```JavaScript
    for(var i of array){
        console.log(i)
    }
    //array[0]
    //array[1]
    ...
    //使用Symbol.iterator获取对象的@@iterator内部属性
    var it = array[Symbol.iterator]();
    it.next()//{value:array[0],done:false}
    ...
    it.next()//{done:true}
    ```

### 混合对象“类”
#### 类理论
- 类的设计模式
    + 类是一种设计模式，不是必须的编程基础
- JavaScript中的类
    + JavaScript中没有类，提供了一些近似类的语法

#### 类的机制
- 建造
    + 类和实例的关系
- 构造函数
    + 构造类实例的一个特殊类方法

#### 类的继承
- 多态
    + 虚拟多态，相对多态
- 多重继承


#### 混入
- 显式混入
- 隐式混入

### 原型
### 行为委托
### ES6中的class
## 类型和语法
### 类型
### 值
### 原生函数
### 强制类型转换
### 语法
### 混合环境JavaScript
## 异步和性能
### 异步的现在和将来
### 回调
### Promise
### 生成器
### 程序性能
### 性能测试与调优
### asynquence库
### 高级异步模式
## 起步上路
### 深入编程
### 深入JavaScript
## ES6及更新版本
### ES的现在与未来
### ES6语法
### 代码组织
### 异步流控制
### 集合
### 新增API
### 元编程
### ES6之后






