# 轻量级微服务架构实践

### 基础设施

- Kubernetes Dashboard [https://k8s.anoyi.com](https://k8s.anoyi.com)

```
# 登录令牌

eyJhbGciOiJSUzI1NiIsImtpZCI6IiJ9.eyJpc3MiOiJrdWJlcm5ldGVzL3NlcnZpY2VhY2NvdW50Iiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9uYW1lc3BhY2UiOiJrdWJlLXN5c3RlbSIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VjcmV0Lm5hbWUiOiJ2aXNpdG9yLXVzZXItdG9rZW4taHF4bWgiLCJrdWJlcm5ldGVzLmlvL3NlcnZpY2VhY2NvdW50L3NlcnZpY2UtYWNjb3VudC5uYW1lIjoidmlzaXRvci11c2VyIiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9zZXJ2aWNlLWFjY291bnQudWlkIjoiMzY4M2I2NmMtODI5Ni0xMWU4LWE4YTMtMDAxNjNlMGM1YmQxIiwic3ViIjoic3lzdGVtOnNlcnZpY2VhY2NvdW50Omt1YmUtc3lzdGVtOnZpc2l0b3ItdXNlciJ9.TnV3EBLW_pangBYLKC7XNRKDR74Z7x-HvzrRDu12rk4mgAlfNgl_vnNkdrDNovMgyFzvDnmvl-cPmJRC9GNFkaGVv39LIxK2Q_NC93XitD1J4aS5qLflWSuuPyeIyjg2ngAt76PMVWeHXZzS4RMjS0KzBdIOusPOBL9YbIxJVqwcU5KVe_i1LRUgHxlhpt9kvX7WPliYCMy7NU0qQafl4oBt-MPkKJy9VcAx5xlJpqK0zXoAK0x4IN1fUfo3veRgKtB8iE7cEJhbkizXxrydOBbT2bm2aBPyq1_DisC3I3rKAbsXcmFLaFJTCmfcW0TN5M3CSrd-UdPrIcjkjMc9FA

```
- Artifactory - Maven Repository [https://mvn.anoyi.com](https://mvn.anoyi.com)
- Jenkins - CI/CD [https://ci.anoyi.com](https://ci.anoyi.com)
- Yapi - Application API Management [https://api.anoyi.com](https://api.anoyi.com)
- Grafana - All Stack Monitoring [Cluster](https://grafana.anoyi.com/dashboard/db/cluster?orgId=1) | [Pods](https://grafana.anoyi.com/dashboard/db/pods?orgId=1)

### 应用层

**网关 [micro-core-gateway](https://github.com/ChinaSilence/micro-core-gateway)**

核心技术 Spring Cloud Gateway

**用户服务 micro-server-user**



### 技术交流

QQ 群：481678152
