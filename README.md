# Go 后端学习之旅

## 书籍

## 阶段一：Go 基础与环境搭建
- [x] 相关书籍
    - [x] Learning Go
    - [x] Go Programming Language
- [x] 搭建本地的 Go 开发环境
    - [x] 安装 Go SDK
    - [x] 配置 Neovim + gopls
    - [x] dlv 调试
- [x] 掌握 Go 语言基础语法
    - [x] 变量
    - [x] 数据类型
    - [x] 运算符
    - [x] 控制结构
    - [x] 函数
- [x] 学习 Go 的包管理和模块化 (go mod)
- [x] 理解错误处理 (error 和 panic/recover)
- [x] 掌握并发编程基础
    - [x] goroutine
    - [x] channel
    - [x] Context
    - [x] Mutex
    - [x] WaitGroup
    - [x] select
- [x] 理解面向接口编程 (interface)
- [x] 学习 Go 的测试框架 (testing)
- [x] 熟悉 Go 标准库常用包
    - [x] fmt
    - [x] os
    - [x] io
    - [x] strings
    - [x] strconv
    - [x] time
- [x] 泛型
- [ ] 源码阅读
  - [ ] `fmt` 包：了解格式化输出的实现
  - [ ] `io` 包：了解输入输出的抽象
- 常见错误：
  - [x] [Traps, Gotchas, and Common Mistakes for New Golang Devs](http://devs.cloudimmunity.com/gotchas-and-common-mistakes-in-go-golang/index.html)

## 阶段二：网络编程与 Web 框架
- [ ] 掌握网络编程基础
  - [ ] TCP/IP 协议
  - [ ] HTTP 协议
- [ ] 学习 Go 网络编程
  - [ ] net 包
  - [ ] http 包
- [ ] 选择 Web 框架
  - [ ] gin
  - [ ] echo
  - [ ] mux
- [ ] 理解路由、中间件、请求处理、响应处理
- [ ] 学习 JSON 处理 (encoding/json)
- [ ] 学习 HTML 模板引擎 (html/template)
- [ ] 理解 RESTful API 设计原则
- [ ] 库使用
  - [ ] `net/http` (Go 标准库)
  - [ ] 选择一个 Web 框架
- [ ] 源码阅读
  - [ ] `net/http` 包：理解 HTTP 服务器如何工作
  - [ ] 选择的网络框架的源码
- [ ] 编写简单的 HTTP 服务，熟悉 Web 开发流程
- [ ] 学习 API 文档编写 (例如 Swagger)

## 阶段三：数据库与 ORM
- [ ] 掌握 SQL 基础
  - [ ] CRUD
  - [ ] JOIN
  - [ ] 索引
- [ ] 学习关系型数据库或 NoSQL 数据库
  - [ ] MySQL
  - [ ] PostgreSQL
  - [ ] MongoDB
- [ ] 理解数据库连接池
- [ ] 学习 ORM 框架
  - [ ] gorm
  - [ ] xorm
- [ ] 数据模型定义
- [ ] 学习数据库迁移
- [ ] 库使用
  - [ ] `database/sql` (Go 标准库)
  - [ ] 选择一个 ORM 框架
  - [ ] 数据库驱动程序（例如：`github.com/go-sql-driver/mysql` 或 `github.com/lib/pq`）
- [ ] 源码阅读
  - [ ] ORM 框架的源码
  - [ ] `database/sql` 包
- [ ] 选择一个数据库，并尝试连接和操作

## 阶段四：测试、部署和微服务
- [ ] 掌握单元测试和集成测试
- [ ] 理解依赖注入 (DI)
- [ ] 学习 Docker 和 Docker Compose
- [ ] 理解 CI/CD (GitHub Actions, Jenkins)
- [ ] 学习微服务架构概念
- [ ] 理解 API 网关、服务发现和负载均衡
- [ ] 学习消息队列
  - [ ] RabbitMQ
  - [ ] Kafka
- [ ] 库使用
  - [ ] `testify/assert`
  - [ ] 选择一个 API 网关/服务发现框架
- [ ] 源码阅读
  - [ ] 选择的微服务框架源码
  - [ ] docker/docker 的源码
- [ ] 编写简单的微服务，学习微服务设计的实践
- [ ] 尝试使用 Docker 部署你的应用

## 阶段五：深入学习与拓展
- [ ] 深入学习 Go 语言的内存模型和并发机制
- [ ] 学习性能优化技巧
- [ ] 学习设计模式
- [ ] 理解缓存、限流、熔断等技术
- [ ] 库使用
  - [ ] `uber-go/fx` (依赖注入)
  - [ ] `go-redis/redis/v8` (Redis 客户端)
  - [ ] `prometheus/client_golang` (监控)
- [ ] 源码阅读
  - [ ] Go Runtime 的源码 (调度器、垃圾回收等)
- [ ] 关注 Go 社区的最新动态，参与开源项目
- [ ] 不断学习新技术和新工具

