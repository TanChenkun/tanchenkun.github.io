---
layout: post
title: border-radius详解
date: 2019-04-23
tags: Css 前端开发
categories: 技术
---

border-radius圆角边框是CSS3的新属性，以前网页设计开发中要实现元素的圆角边框，通常是用背景图片来实现的。现在我们只需要给元素添加border-radius属性即可。
![border-radius原理](/assets/img/posts/radius/1.png)

## 一、语法
1.单值,
```css
border-radius:6px;
```
表示元素四个方向的圆角大小都是6px，即每个圆角的“水平半径”和“垂直半半径”都设置为6px


2.四个属性值
```css
border-radius:10px 20px 30px 40px;
```
分别表示左上角、右上角、右下角、左下角的圆角大小（顺时针方向）。
![四个属性值](/assets/img/posts/radius/2.png)


3.三个属性值
```css
border-radius:10px 30px 60px;
```
第一个值表示左上角，第二个值表示右上角和左下角（对角），第三个值表示右下角。
![三个属性值](/assets/img/posts/radius/3.png)


4.两个属性值
```css
border-radius:20px 40px;
```
第一个值表示左上角和右下角，第二个值表示右上角和左下角。
![两个属性值](/assets/img/posts/radius/4.png)


5.斜杠二组值
```css
border-radius:100px/40px;
border-radius:60px 60px 60px 60px/100px 100px 60px 60px;
```
第一组值表示水平半径，第二组值表示垂直半径，每组值也可以同时设置1到4个值，规则与上面相同。
![斜杠二组值100/40](/assets/img/posts/radius/5.png)
![斜杠二组值](/assets/img/posts/radius/6.png)











