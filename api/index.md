# HARBORS API LIST

1. 1. [CORE](/api/core) - HARBORS core

    > 1.1 [Class](/api/core/class): 与继承等相关的方法都在这个类中。需要继承其他方法的也可以改写这个类来实现
  
    > 1.2 [Debugger](/api/core/debugger): 初始化一系列调试方法
  
    > 1.3 [Request](/api/core/request): 这个集合内的所有方法会在接受请求的时候复制到http的request对象上
  
    > 1.4 [Response](/api/core/response): 每个请求的response对象将从这里开始创建
  
    > 1.5 [Server](/api/core/server): 负责监听端口，接收用户请求等的入口
  
    > 1.6 [VHost](/api/core/vhost): 虚拟主机，创建主机负责接收server传递出来的请求

2. 2. [ROUTE](/api/route) - Responsible for handling the routing rules

    > 2.1 [AutoRouter](/api/route/autorouter): 在Router基础上增加自动返回静态文件的功能
    
    > 2.2 [Router](/api/route/router): 根据路由规则处理链接以及寻找相应的处理程序

3. 3. [PROCESS](/api/process) - Some process control
   
    > 3.1 [Cluster](/api/process/cluster): 负责生成，存储，更新当前VHost对象内的session
    
    > 3.2 [Sync](/api/process/sync): 流程处理

4. 4. [EXTENSION](/api/extension) - Extension of the class

    > 4.1 [Config](/api/extension/config): 负责解析传入的js对象，并将根据规则创建相应的服务器对象
    
    > 4.2 [Session](/api/extension/session): 负责生成，存储，更新当前VHost对象内的session
    
    > 4.3 [FileSession](/api/extension/session): 在session类构建的基础上，实现文件存储session的类

5. 5. [TOOLS](/api/tools) - Tools

    > 5.1 [Directory](/api/tools/directory): 文件夹相关的一些功能封装
    
    > 5.2 [String](/api/tools/string): 字符串相关的一些功能封装