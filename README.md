# Chinanet

Derive from [gfwlist](https://github.com/gfwlist/gfwlist) and [china ip list](https://github.com/17mon/china_ip_list)

## 目标

在域名和IP两个方面，尽最大努力区分Chinanet和Internet，再针对性的部署相应的域名解析方案和路由方案

最终达到近似无人值守式对抗GFW的黑名单升级事件

## 域名

按照一定策略对域名进行分类，针对不同类别的域名采取不同的解析策略

### 分类

1. A.（超大概率非中国区运营域名）TLD，顶级域，去除`com.`和`cn.`
1. B.（GTLD例外清单）根据经验，使用了A类GTLD但在中国区运营的域名
1. C.（显式屏蔽清单）从gfwlist中提取出所有`com.`域名
1. D.（例外新增清单）gfwlist中尚未收录的域名

### 策略

* A. 非中国区解析
* B. 默认解析
* C. 非中国区解析
* D. 非中国区解析

## IP

以china ip list为准
