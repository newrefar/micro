# 轻量级微服务架构实践

### 基础设施

- Kubernetes Dashboard [https://k8s.anoyi.com](https://k8s.anoyi.com)

```
# 登录令牌

eyJhbGciOiJSUzI1NiIsImtpZCI6IiJ9.eyJpc3MiOiJrdWJlcm5ldGVzL3NlcnZpY2VhY2NvdW50Iiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9uYW1lc3BhY2UiOiJrdWJlLXN5c3RlbSIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VjcmV0Lm5hbWUiOiJ2aXNpdG9yLXVzZXItdG9rZW4tdHdodjIiLCJrdWJlcm5ldGVzLmlvL3NlcnZpY2VhY2NvdW50L3NlcnZpY2UtYWNjb3VudC5uYW1lIjoidmlzaXRvci11c2VyIiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9zZXJ2aWNlLWFjY291bnQudWlkIjoiMDY4YTRlN2UtOGVlZS0xMWU4LWJiYTAtMDAxNjNlMGM1YmQxIiwic3ViIjoic3lzdGVtOnNlcnZpY2VhY2NvdW50Omt1YmUtc3lzdGVtOnZpc2l0b3ItdXNlciJ9.EgPE1QSCFoh9mOCtwC9iMivPCcWa2M549PyoOgAxAKR6yYNa2pZAkfzb-I2dLvmxz7yi1A2jQLzDw_fEsgmQZi-WSyWA7xA5y-qBDlWjzDc5gHwbstdcClUM4mZUldxls4qDWwfLrIAbUfXpK-kYuzTGFCvkGYTTWNgTJ9kUxhyJEK3lU1b84lZzwEI1JMTYttpXqs1Cklvetp-y0WkVSA53PqdflUbXB6fZX_Iyo-oX75kMn1hg3LdaVhx8zoR36Op0IDKZul_1O1rRE3GbcTmNo48q1HngnO8Yi6t1BKc5ln4FRMEWT6lPgQNwcFIFWDru8XzKAMSmP0AoJlcMyA

```
- Artifactory - Maven Repository [https://mvn.anoyi.com](https://mvn.anoyi.com)

```
账号  user
密码  anoyi.com
```

- Jenkins - CI/CD [https://ci.anoyi.com](https://ci.anoyi.com/blue/pipelines)

```
无需登录认证
```

- Yapi - Application API Management [https://api.anoyi.com](https://api.anoyi.com)

```
账号  user@anoyi.com
密码  anoyi.com
```

- Grafana - All Stack Monitoring [Nodes](https://grafana.anoyi.com/d/fa49a4706d07a042595b664c87fb33ea/nodes?orgId=1) | [Pods](https://grafana.anoyi.com/d/ab4f13a9892a76a4d21ce8c2445bf4ea/pods?orgId=1)

```
账号  viewer@anoyi.com
密码  anoyi.com
```

- Kibana - All Stack Logging [https://log.anoyi.com/](https://log.anoyi.com/)

```
无需登录认证
```

- SCCA - Spring Boot 配置管理中心 [https://conf.anoyi.com/](https://conf.anoyi.com/)

```
账号 user
密码 anoyi123
```

> 请文明使用，共建良好环境！

----

### 应用层

**网关** -> [micro-core-gateway](https://github.com/ChinaSilence/micro-core-gateway)

> 核心技术 Spring Cloud Gateway，作用：后端服务路由、统一身份认证、限流等

**用户服务** -> [micro-server-user](https://github.com/ChinaSilence/micro-server-user)

> 用户信息管理

**抖音服务** -> [micro-server-douyin](https://github.com/ChinaSilence/micro-server-douyin)

> 抖音数据爬取

**抖音服务** -> [micro-node-douyin](https://github.com/ChinaSilence/micro-node-douyin)

> 抖音加密算法解密，使用 NodeJS 提供参数加密值

**即时通信** -> micro-server-websocket

> WebSocket 服务，双向通信

-----

### 技术交流

QQ 群：481678152
