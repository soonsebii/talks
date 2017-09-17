# talks
Materials

* [20161025_event_loop.zip](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/simenkid/talks/tree/master/20161025_event_loop): Node.js 線上讀書會分享 Event Loop 與 EventEmitter, 內含 demo examples  
  - 修正投影片 p28 標題為 Run With Another Process，原為 Run With Another Thread。謝謝 [@ysarron](https://github.com/ysaaron) 提醒。
  
  
# 01_server.js
```
$ node 01_server.js &
$ pidof node | xargs pstree -h -ap
node,6189 01_server.js
  ├─{V8 WorkerThread},6191
  ├─{V8 WorkerThread},6192
  ├─{V8 WorkerThread},6193
  ├─{V8 WorkerThread},6194
  └─{node},6190
```
