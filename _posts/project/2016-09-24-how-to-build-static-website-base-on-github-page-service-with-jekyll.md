---
layout: post
title: 基于github page 快速搭建blog
category: project
description: 极简可用教程。
---
# 前提：
- 会配置dns
- 会使用git和github.com
- 懒

# 步骤1：  申请pages服务，
登陆github后按照常规新建一个仓库，假设你的github用户名是 _ABC_， 那仓库名就设置为 _ABC.github.io _。  然后将仓库克隆到你本地。

# 步骤2：  绑定域名【可选】
在 _ABC.github.io_仓库里新增一个文件，文件名 _CNAME_， 文件内容为你的域名，如ABC.COM。  
  
设置你域名的dns信息如下：

> host:www.ABC.com   type: CNAME   value: ABC.github.io
> host:@.ABC.com     type: a       value: 192.30.252.154
> host:@.ABC.com     type: a       value: 192.30.252.153

# 步骤3： 安装jekyll到你的本机
好吧，折腾的做法。。。。事实上不需要本机安装它就可以解决问题
—
快速的做法是： 打开知乎、或者百度、google 搜索一些你觉得可用的github page网页，然后clone 下他的仓库文件。将文件存放到 _ABC.github.io_ 的仓库里
然后提交修改github 。 

--— 
好了，你已创建了你自己的blog了，记得删除掉不是你的文章页面哦

# 步骤4： 了解一下jekyll的代码组成架构即可

> _config.yml 配置文件
> _layouts 网站的布局目录，
> _posts  这个目录存放的都是你的文章，文章格式为markdown格式，后缀md
> _sites  这个不用管，用不上。

跟我们有关系的也就是post目录了，以后你写好每篇文章都存放在这里既可，其他的无需理会，_内容为主，先用了再说，如果真合适，能坚持下去了，在自定义也不迟_


ps： 如果你用ulysess的话，可以直接将 post目录 关联进软件，直接用它来新增、删除、修改、管理你的文章。 完了后git 提交一下即可。


