# psub
利用CF Worker搭建的反代订阅转换工具，通过随机化服务器地址和节点账号密码，解决用户转换订阅的隐私问题

### 演示网站
https://psub.888005.xyz

### 视频教程
https://youtu.be/X7CC5jrgazo

环境变量名：`BACKEND`

KV或R2变量名：`SUB_BUCKET`

假设我们有两个订阅链接：

- https://example1.com/sub1
- https://example2.com/sub2

当 `RENAME_NODES` 为 false 时，节点名称保持原样：

- 节点1
- 节点2
- 快速节点
- 美国节点

当 `RENAME_NODES` 为 true 节点名称会被修改，添加订阅源的信息。例如：

- 节点1-sub1
- 节点2-sub1
- 快速节点-sub2
- 美国节点-sub2

在这个例子中：
- "sub1" 是从 "https://example1.com/sub1" 提取的
- "sub2" 是从 "https://example2.com/sub2" 提取的

### 支持反代转换的协议
 - shadowsocks
 - shadowsocksR
 - vmess
 - trojan
 - vless(取决于后端)
 - hysteria(取决于后端)

### 打赏
请我喝矿泉水：[全专线中专机场AFF链接](http://b.880805.xyz/)

请我喝桶装水：[搬瓦工美国CN2 GIA线路AFF链接](https://bwg.880805.xyz/)
