### 介绍说明

Kubernetes 集群内部各种资源部署的配置文件。

### 应用列表

+ application
  + artifactory: Maven 私服
  + fluentd: 集群统一日志收集
  + jenkins: 持续集成、持续交付
  + kibana: 日志数据可视化分析
  + kubernetes-dashboard: Kubernetes 管理面板
  + kubernetes-heapster: Kubernetes 集群监控
  + yapi: 服务 API 文档管理平台
+ database
  + elasticsearch: 存储日志数据
  + mongo: 存储 Yapi 数据
  + mysql: 微服务应用层数据
  + redis: 分布式 session / 缓存
+ dynamic-volume: Kubernetes NFS 动态存储

### 使用方式

1、创建 kubernetes NFS 动态存储（注意修改 `nfs-provisioner.yaml` 文件，指定提供存储的服务器及挂载路径）
```
kubectl create -f dynamic-volume/
```

2、application 和 database 部署

- pvc.yaml: 存储消费
- secret.yaml: 加密存储
- config.yaml: 普通配置
- init.yaml: 服务部署前的初始化操作
- deployment.yaml: 部署应用
- service.yaml: 创建服务，暴露给外部

执行顺序： pvc -> secret -> config -> init -> deployment -> service (不同应用包含的部署文件可能不同)
