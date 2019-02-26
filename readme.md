### 参考文档
- 说明文档：https://socket.io/get-started/chat/
- 仓库：https://github.com/socketio/socket.io/blob/master/examples/chat/README.md

### 整理下思路
1. 每一个user都会创建一个io，并且可以将他的昵称放在sockect session下；
2. 每一个user发了一个消息，都需要通知服务区，服务器broadcast给所有的成员；
3. 每一个user加入聊天室，离开，都需要通知服务器，服务广播给所有的成员；
4. 聊天室里面的人数需要统计；放在数据库或者内存，磁盘都可以；


### TODO
1. 断开重链；
2. 离线消息缓存；
3. 消息漫游；
4. 性能：丢包率，及时性