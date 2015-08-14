# Pholcus 使用手册

![logo](images/icon.png)

Pholcus（幽灵蛛）是一款纯Go语言编写的高并发、分布式、重量级爬虫软件，支持单机、服务端、客户端三种运行模式，拥有Web、GUI、命令行三种操作界面；规则简单灵活、批量任务并发、输出方式丰富（mysql、mongodb、csv、excel等）、有大量Demo共享；同时她还支持横纵向两种抓取模式，支持模拟登录和任务暂停、取消等一系列高级功能。

![模块构成](images/project.png)

#### 框架特点
 1. Pholcus（幽灵蛛）以高效率，高灵活性和人性化设计为开发的指导思想；

 2. 支持单机、服务端、客户端三种运行模式，即支持分布式布局，适用于各种业务需要；
 
 3. 支持Web、GUI、命令行三种操作界面，适用于各种运行环境；
 
 4. 支持mysql/mongodb/csv/excel等多种输出方式，且可以轻松添加更多输出方式；
 
 5. 采用surfer高并发下载器，支持 GET/POST/HEAD 方法及 http/https 协议，同时支持固定UserAgent自动保存cookie与随机大量UserAgent禁用cookie两种模式，高度模拟浏览器行为，可实现模拟登录等功能；

 6. 服务器/客户端模式采用teleport高并发socketAPI框架，全双工长连接通信，内部数据传输格式为JSON；
 
 7. 对采集规则进行了精心设计，规则灵活简单、高度封装，用于通用方法集与大量Demo，让你轻松添加规则；
 
 8. 支持横纵向两种抓取模式，并且支持任务暂停、取消等操作。



#### 第三方依赖包

```
go get "github.com/henrylee2cn/surfer"
go get "github.com/henrylee2cn/teleport"
go get "github.com/PuerkitoBio/goquery"
go get "github.com/bitly/go-simplejson"
go get "github.com/henrylee2cn/mahonia"
go get "github.com/andybalholm/cascadia"
go get "github.com/lxn/walk"
go get "github.com/lxn/win"
go get "github.com/tealeg/xlsx"
go get "github.com/go-sql-driver/mysql"
go get "gopkg.in/mgo.v2"
<以下需翻墙下载>
go get "golang.org/x/net/html"
go get "golang.org/x/text/encoding"
go get "golang.org/x/text/transform"
```
> *<font size="2">（在此感谢以上开源项目的支持！）</font>*



#### 开源协议

Pholcus（幽灵蛛）项目采用商业应用友好的[Apache License v2](https://github.com/henrylee2cn/pholcus/blob/master/doc/license.txt).发布

