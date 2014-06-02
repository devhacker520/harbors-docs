# [CORE](/api/core) - HARBORS core

1. [Class](/api/core/class): 与继承等相关的方法都在这个类中。需要继承其他方法的也可以改写这个类来实现
  
2. [Debugger](/api/core/debugger): 初始化一系列调试方法
  
3. [Request](/api/core/request): 这个集合内的所有方法会在接受请求的时候复制到http的request对象上
 
4. [Response](/api/core/response): 每个请求的response对象将从这里开始创建
  
5. [Server](/api/core/server): 负责监听端口，接收用户请求等的入口
  
6. [VHost](/api/core/vhost): 虚拟主机，创建主机负责接收server传递出来的请求

