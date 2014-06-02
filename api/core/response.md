# harbors.Response

基础类

每个请求的response对象将从这里开始创建

- **Response.end(data, encoding)**

    > @data {String|Buffer}
    
    > @encoding {String}
    
    > 结束一个用户请求，并将数据返回给客户端，详细用法参考原生nodejs。
    
- **Response.write(chunk, encoding)**

    > @chunk {String|Buffer}
    
    > @encoding {String}
    
    > 将数据片段返回给客户端，详细用法参考原生nodejs。
    
- **Response.writeHead(statusCode, reasonPhrase, headers)**

    > @statusCode {Number}
    
    > @reasonPhrase {String|Buffer}
    
    > @headers {String}
    
    > 同上，详细用法参考原生nodejs。
    
- **Response.writeHeader(statusCode, headers)**

    > @statusCode {Number}
    
    > @headers {Object}
    
    > 返回一个完整的header给客户端
    
- **Response.addTrailers(headers)**

- **Response.removeHeader(name)**

- **Response.getHeader(name)**

- **Response.setHeader(name, value)**

- **Response.setCookie(name, value, option)**

- **Response.setTimeout(msecs, callback)**

- **Response.getSent()**

- **Response.setSession(name, value)**

- **Response.render(fileName, option)**

    
