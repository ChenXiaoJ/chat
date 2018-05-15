# chat
在线答疑
測試
嗯嗯那

npm run deploy:production
```

Redis:
-----------------
`cd /etc/redis & redis production.conf`

restart redis:
```
  redis-cli save  // [ 不然会丢失可能10分钟的数据 ]
  kill -9 PID   // [ PID就是这个redis-server process的id ]
  redis-server production.conf  // [ 启动redis ]

  或 redis-cli shutdown  // [ 用auth登录客户端关闭 ]

Logs:
------------------
Logs in the prod and staging are located in ~/dev/log/passenger.log。 `tail -f ~/dev/log/passenger.log` to view the log in the real time
