# harbors.Request

方法集合

这个集合内的所有方法会在接受请求的时候复制到http的request对象上。

- **Request.getHeaders(name)** 

    > @name {String}
    
    > @returns {String|Array|Number|Object}
    
    > 传入需要获取的headers名字，将返回该字段相符的header。如果不传入，默认则返回整个header对象。
    
- **Request.getURL()**

    > @returns {String}
    
    > 返回当前用户正在访问的url地址
    
- **Request.getGetParam(name)**

    > @name {String}
          
    > @returns {String|Number|Object}
    
    > 传入需要的get参数名，返回对应的值。如果不传入，默认返回所有get参数对象。
    
- **Request.getPostParam(name)**

    > @name {String}
          
    > @returns {String|Number|Object}
    
    > 传入需要的post参数名，返回对应的值。如果不传入，默认返回所有post参数对象。
    
    > **注意：** 需要当前VHost允许接受post数据才能使用此方法。
    
- **Request.getFiles(name)**

    > 同上
    
- **Request.getCookie(name)**

    > @name {String}
    
    > @returns {String|Number|Object}
    
    > 传入需要获取的cookie名字，将返回该字段相符的cookie。如果不传入，默认则返回整个cookie对象。
    
- **Request.getSession(name)**

    > 同上
    
    > **注意**：需要VHost中开启相应的session功能。