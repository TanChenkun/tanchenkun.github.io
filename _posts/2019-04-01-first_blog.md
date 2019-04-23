---
layout: post
title: Js解决app-input框聚焦问题
date: 2019-04-01
tags: JavaScript 前端开发
categories: 技术
---

 JS实现focus()获得文本框焦点后,光标位置跳到文本末尾,之前在工作中有遇到类似微信聊天窗口的功能开发，采用的是angular 7.0 + ionic 4，功能难点在于表情框的实现-表情的多次选择后，点击关闭表情按钮，input框聚焦后光标不会直接在内容末尾处出现，影响用户体验。

### 介绍

```
  setSelectionRange()

```
  The HTMLInputElement.setSelectionRange() method sets the start and end positions of the current text selection in an element.

  setSelectionRange()方法是作用在input元素上的，其次，这个方法可以为当前元素内的文本设置备选中范围（selection）。简单来说，就是可以通过设置起始于终止位置，来选中一段文本中的一部分。值得一提的是，在新版中，该方法还接受一个可选参数，这个参数指定的选择的方向。 其使用方式如下：

```

  inputElement.setSelectionRange(selectionStart, selectionEnd, [optional] selectionDirection);

```
- selectionStart：第一个被选中的字符的序号（index），从0开始。
- selectionEnd：被选中的最后一个字符的前一个。换句换说，不包括index为selectionEnd的字符。
- selectionDirection：选择的方向。可选值为forward、backward或none。









