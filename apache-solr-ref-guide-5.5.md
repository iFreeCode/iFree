# Apache Solr 介绍
## 快速开始
### 安装Solr
#### 启动Solr
##### 开启服务
`$ bin/solr start`

`bin\solr.cmd start`

Solr会在8983端口开启服务
##### 停止服务
`$ bin/solr stop -p 8983`
##### 开启Solr例子
`$ bin/solr -e techproducts`
##### 检测Solr运行状态
`$ bin/solr status`
##### 创建主服务
如果你没有通过配置案例启动Solr，你需要创建一个Core来索引和搜索。你可以按照如下：
`$ bin/solr create -c <name>`

