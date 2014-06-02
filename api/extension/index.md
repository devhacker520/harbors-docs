# [EXTENSION](/api/extension) - Extension of the class

1. [Config](/api/extension/config): 负责解析传入的js对象，并将根据规则创建相应的服务器对象
    
2. [Session](/api/extension/session): 负责生成，存储，更新当前VHost对象内的session
    
3. [FileSession](/api/extension/session): 在session类构建的基础上，实现文件存储session的类