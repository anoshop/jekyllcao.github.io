---
layout: post
title: 批量查询域名注册状态（俗称扫米）工具
category: project
description: 支持500+个域名后缀，可自由扩展，不限线程
---




## Update：
针对com、net、org等有更强劲的后缀，可以考虑使用高性能版本。
![][image-1]
> 实测记录： 
> real 0m9.767s 
> user 0m0.415s 
> sys 0m0.632s 


目前只编译了 mac 系统可用的版本 
http://104.131.133.121/mac\_speed 
放到跟 mac 同目录即可，
参数中的 缓存时间为 微妙，即1000 微秒 = 1秒。


 
## 功能：
根据字典批量查询域名是否可以注册

## 下载

**[http://104.131.133.121/BAT.zip][1]**

## GIF演示
![演示][image-2]
## 用法：

执行：
**程序名 + 空格 +域名后缀 +空格+ 字典文件名 + 空格+ 超多线程启动间隔时间(秒)**

结果汇总：
程序根目录下会有  **域名后缀-时间-succ.txt** 文件生成，该文件为可用结果集合。

### 各大系统使用示例：
**Window 用户**，有2种用法：
a、直接执行startWindow.bat 文件，
b、用cmd进入到文件所在目录，然后输入
 `window.exe com 3py.txt 3 `

**Linux用户**：
请从终端进入文件所在目录，然后输入 
`./linux com 3py.txt 3 `


**OSX 用户**：
请从终端进入文件所在目录，然后输入 
`./mac com 3py.txt 3 `


## 配置修改
### 字典增减：
可以在dict目录增加任意文本文件，一行一个字符串


### 域名后缀增减：
直接编辑data目录下的tld.org.json

## 作者:Eric.c via  http://sunorg.net
## 授权：随意用，方便就挂个友情链接，不方便就随意



[1]:	[http://104.131.133.121/BAT.zip] "【点这里下载，下载地址如失效不补】"

[image-1]:	http://104.131.133.121/domainSpeed.gif "高速版本"
[image-2]:	http://104.131.133.121/domain.gif "演示"