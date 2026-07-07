# SaaS-Zero Etcd 调试工具

服务注册中心。开发环境通过 etcd 管理服务发现与配置分发。

## 启动

```bash
# 启动 etcd 服务
cd apps/saas-zero-etcd
go run etcd.go
```

## 调试

```bash
# 查看已注册的服务
etcdctl get --prefix ""

# 查看 basedata RPC 注册信息
etcdctl get /basedataservice.rpc --prefix
```

## 连接信息

| 项目 | 值 |
|---|---|
| 版本 | etcd release-3.6.5 |
| 源码 | https://github.com/etcd-io/etcd |
