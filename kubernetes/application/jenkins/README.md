### 常见问题

**1、Jenkins 容器重启后，出现 Error fetching remote repo 'origin'**

解决方法：在新容器里面执行：
```
chown -Rc 0 /var/jenkins_home/workspace/*/.git
```