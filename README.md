# 更新说明：

clash适配了trojan,修复了个别协议无法识别报错

新增生成二维码

# 功能说明：

节点转换成订阅，并且能够一直存储

方便多订阅管理，个人搭建使用

解决安全问题预防被偷节点

目前支持v2ray通用的格式和clash格式

v2ray格式通用的软件已测有下:v2rayn 小火箭 等，还有一些没用过不知名


# 安装说明：

## 拉取docker镜像

```docker pull jaaksi/sublink:1.0```

## 启动docker

```docker run -p 5000:5000 -d jaaksi/sublink:1.0```

如果要自定义端口 -p 5000:5000左边的5000改成自定义右边为固定如:8000:5000

那么公网加8000端口即可访问

默认账户密码都是admin

# clash配置说明：

目前适配了vless,vmess,ssr,ss,trojan协议，其中vmess中的传输只支持ws和默认

vless则是reality

这些并未测试使用，如果发现连接无效问题请找我反馈

# clash规则说明：

我提供了一个默认带分流规则，提供了策略组变量：auto

在proxy-groups下面的proxies写上auto可自动获取节点名称

如果你不明白这是什么意思你就不用动默认规则

本人电报联系和投喂：@toutie_1