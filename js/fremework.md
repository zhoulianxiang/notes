# 简易数据库网络架构搭建

之前做过的一个系统思路简单小结，只需要大致掌握JavaScript即可完成。

## 操作系统
- Linux

## 数据库
- PostgreSQl
  - https://www.postgresql.org
  - http://www.postgres.cn/docs/10/index.html 中文手册
  - 按照业务逻辑设计数据库/表即可

## 后端
- Nodejs
  - https://nodejs.org/en/
  - https://nodejs.org/en/download/
  - https://nodejs.org/en/download/package-manager/
  - https://nodejs.org/dist/v8.11.3/node-v8.11.3.tar.gz
- Express
  - http://www.expressjs.com.cn/
  - http://www.expressjs.com.cn/starter/installing.html
    - 这一步直接生成了后端框架，之后的代码就是基于这个框架目录添加/修改
    - 通常没有特别需求，按照示例输入指令就可以完成了
- node-postgres
  - https://github.com/brianc/node-postgres
  - https://node-postgres.com
  - https://node-postgres.com/guides/project-structure
    - 这一页是参考示例，直接照抄就好了
    - _主要的数据库操作都是在这一部分完成，比如我们需要查询/插入/删除/修改的一些操作_

## 前端
- JavaScript/JQuery/Bootstrap/Ajax
  - 可以很简单的生成网页
  - 和服务器进行数据交互
  - _这一部分的开发量要看我们有多少页面需要编写_

## 总结

- 数据库设计需思路清晰、简洁
- 框架的生成直接按照示例或者标准步骤即可
- 需要编写代码的是两个部分，也是**主要的工作量**
  - 后端和数据库交互代码，可以简单的认为添加处理函数
  - 前端页面开发，可以简单的认为普通的网页开发
  
# END
