---
title: ' 图床（imhost）—— PicGo+腾讯云对象存储COS+Typora'
date: 2023-3-17T10:59:04+08:00
image: ""
tags:  ["PicGo","COS","imhost","Tutorial"]
description:  'Web 工具使用技巧'
lastmod: '2023-10-17'
categories: 
    - "Web"
    - "Tool"
---

# 图床（imhost）—— PicGo+腾讯云对象存储COS+Typora

## 概念介绍

1. 图床（Imhost）：简单来说，将图片上传服务器，每张图片获得一个连接。在任意联网设备访问此连接，即可显示图片，主要用于`.html`，`.md`等文件中。
2. [Tencent COS](https://curl.qcloud.com/i4ly02I3)：提供提供对象存储的服务，可以储存多种类型文件。
3. Typora：一种`markdown`编辑器

## **工具**

 1. [Picgo](https://github.com/Molunerfinn/PicGo/releases)
 2. [腾讯云COS（对象存储）](https://console.cloud.tencent.com/cos)
 3. [Typora](typora.io)

## **操作步骤**
### **购买腾讯云COS资源包**
>访问：https://curl.qcloud.com/i4ly02I3，购买资源包
### **PicGo设置**
1. 创建储存桶🧳：
    - 名称：例如test-给定的一串数字
    - 公有读私有写（必须共有读，否则图片无法加载）
2. 创建密钥🔑
    - 使用现有的，或者创建
    - 获得APPID、Secretld、DecreKey
3. 从上面Github的地址下载PicGo
4. 在PicGo中设置
    - 图床版本选择V5(选择V4则无法使用，原因不明)
    - APPID、Secretld、DecreKey为上面提到的密钥界面提供的三个值
    - 设定储存空间名：为创建储存桶的名称，例如：test-给定的一串数字
    - 储存区域：创建的储存桶所属区域（）中的内容，例如：ap-nanjing

## Tips

1. 在[Picgo](https://github.com/Molunerfinn/PicGo/releases)图床设置中选择V5，原因不明
2. [Picgo](https://github.com/Molunerfinn/PicGo/releases)设置中：设置`Server`→端口:`36677`（和[Tencent COS](https://console.cloud.tencent.com/cos)匹配）
3. 一切设置正常（[Tencent COS](https://console.cloud.tencent.com/cos)上传图片正常），在PicGo设置中选择时间戳重命名→上传图片→取消
4. 在[Typora](typora.io)设置[Picgo](https://github.com/Molunerfinn/PicGo/releases)作为图床时，在中文环境下设置：PicGo.app，在英文环境下只有PicGo-core，在中文中设置好后再改成英文环境，可行


-----
参考链接🔗

- [腾讯云COS对象存储+PicGo搭建图床教程](https://blog.csdn.net/qq_41684621/article/details/114128635?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-0-114128635-blog-109720624.pc_relevant_paycolumn_v3&spm=1001.2101.3001.4242.1&utm_relevant_index=3)
- [使用PicGo+腾讯云做图床](https://blog.csdn.net/qq_38576299/article/details/109720624?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-109720624-blog-121218444.pc_relevant_paycolumn_v3&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-109720624-blog-121218444.pc_relevant_paycolumn_v3&utm_relevant_index=2)

- [PicGo和腾讯COS搭建图床](https://blog.csdn.net/weixin_44593310/article/details/123910255)

- [手把手教你用Typora自动上传到picgo图床【教程与排坑】](https://www.jianshu.com/p/4cd14d4ceb1d)