---
layout:  post
title:  SHELL错误
date:  2016-10-31
categories:  日志
tag:  SHELL
---


* content
{:toc}


#### /bin/sh^M:bad interperter:No Such file or directory
最近在window下编写脚本，然后通过XShell上传到Centos上面
执行脚本的时候就出现了`/bin/sh^M:bad interperter:No Such file or directory`，
查找资料，是因为windows和linux文件不一样。具体什么不一样，有待考究。

先贴出解决方法：
vim 进到文件里面，输入 set ff=unix 回车，然后保存就可以了
```
vim demo.sh
set ff=unix
wq
```
![样例](/styles/images/shell/sh^m-nosuchfile.png)
