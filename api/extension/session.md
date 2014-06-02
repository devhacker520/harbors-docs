# harbors.Session

基础类

负责生成，存储，更新当前VHost对象内的session

- **Session.update(req, res, cookie, callback)**

- **Session.createCookie(req, res)**

- **Session.completeData(data)**

# harbors.FileSession

扩展类

在session类构建的基础上，实现文件存储session的类

- **Session.setPath(string)**

- **Session.readSession(cookieName, callback)**

- **Session.saveSession(cookieName, session)**

- **Session.create()**