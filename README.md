# Go 后端学习之旅

## 阶段一：Go 基础与环境搭建
- [x] 相关书籍
    - [x] Learning Go
    - [x] Go Programming Language
- [x] 搭建本地的 Go 开发环境
    - [x] 安装 Go SDK
    - [x] 配置 Neovim + gopls
    - [x] dlv 调试
      - `dlv run main.go`
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
    - [x] TCP/IP 协议
    - [x] HTTP 协议
- [ ] 学习 Go 网络编程
    - [ ] net 包
    - [x] http 包
- [ ] 选择 Web 框架
    - [x] gin
    - [ ] gin-contrib: 提供各种常用的中间件，比如用于处理 CORS、JWT 认证等。
    - [x] [air](https://github.com/air-verse/air) 可以在检测到源码改动后，重新构建运行程序。
        - `air init`
        - `air`
    - [ ] echo
    - [ ] mux
- [x] 理解路由、中间件、请求处理、响应处理
- [x] 学习 JSON 处理 (encoding/json)
- [x] 学习 HTML 模板引擎 (html/template)
- [x] 理解 RESTful API 设计原则
- [ ] 源码阅读
    - [ ] `net/http` 包：理解 HTTP 服务器如何工作
    - [ ] 选择的网络框架的源码
- [x] 编写简单的 HTTP 服务，熟悉 Web 开发流程
- [ ] 学习 API 文档编写 (例如 Swagger)

## 阶段三：数据库与 ORM
- [x] 掌握 SQL 基础
    - [x] CRUD
    - [x] JOIN
    - [x] 索引
- [ ] 学习关系型数据库或 NoSQL 数据库
    - [x] MySQL
    - [x] Redis
    - [ ] PostgreSQL
    - [ ] MongoDB
- [ ] 理解数据库连接池
- [ ] 学习 ORM 框架
    - [ ] gorm
    ```go
    // 可以打开 gorm 底层执行的 SQL 语句，便于理解 GORM 行为。
    db, err := gorm.Open(mysql.Open(dsn), &gorm.Config{
        Logger: logger.Default.LogMode(logger.Info), 
    })
    ```
    - [ ] xorm
- [ ] 学习数据库迁移
- [ ] 库使用
    - [ ] `database/sql` (Go 标准库)
    - [ ] `go-redis/redis/v8` (Redis 客户端)
- [ ] 源码阅读
    - [ ] ORM 框架的源码
    - [ ] `database/sql` 包
- [ ] 选择一个数据库，并尝试连接和操作

## 阶段四：测试、部署和微服务
- 书籍:
  - [x] 凤凰架构
  - [x] Cloud Native Go
- [ ] 掌握单元测试和集成测试
- [ ] 理解依赖注入 (DI)
- [x] 学习 Docker 和 Docker Compose
- [x] 理解 CI/CD (GitHub Actions, Jenkins)
- [x] 学习微服务架构概念
- [ ] go-zero
- [ ] micro/micro:
- [x] 理解 API 网关、服务发现和负载均衡
- [ ] 学习消息队列
    - [ ] RabbitMQ
        - [x] https://www.rabbitmq.com/tutorials
    - [ ] Kafka
- [ ] 库使用
    - [ ] `testify/assert`
    - [ ] 选择一个 API 网关/服务发现框架
- [ ] 编写简单的微服务，学习微服务设计的实践
- [ ] 尝试使用 Docker 部署你的应用

## 阶段五：深入学习与拓展
- [ ] 深入学习 Go 语言的内存模型和并发机制
- [ ] 学习性能优化技巧
- [ ] 学习设计模式
- [ ] 理解缓存、限流、熔断等技术
  - [ ] https://github.com/afex/hystrix-go
- [ ] 库使用
    - [ ] `uber-go/fx` (依赖注入)
    - [ ] `prometheus/client_golang` (监控)
- [ ] 源码阅读
    - [ ] Go Runtime 的源码 (调度器、垃圾回收等)
- [ ] 关注 Go 社区的最新动态，参与开源项目
- [ ] 不断学习新技术和新工具

### 其他
- [ ] Viper: 一个强大的配置管理库，支持多种配置文件格式（如 JSON、YAML、TOML 等）。
    - 官网: https://github.com/spf13/viper
- [ ] Zap: 一个高性能的日志库，适合生产环境使用。
    - 官网: https://github.com/uber-go/zap
- [ ] JWT: 使用 dgrijalva/jwt-go 库来处理 JWT（JSON Web Token）。
    - 官网: https://github.com/dgrijalva/jwt-go
- [ ] Swagger: 使用 swaggo/swag 生成 API 文档。
    - 官网: https://github.com/swaggo/swag
- [ ] Testify: 一个强大的测试库，提供了断言、mock 等功能。
    - 官网: https://github.com/stretchr/testify
- [ ] RabbitMQ: 使用 streadway/amqp 库来操作 RabbitMQ。
    - 官网: https://github.com/streadway/amqp
- [ ] etcd-io/etcd:
    - 描述:  一个分布式键值存储，通常用作服务发现和配置管理。
    - 经验值: 了解分布式系统原理、熟悉一致性算法、理解键值存储的原理。
- [ ] prometheus/prometheus:
    - https://yunlzheng.gitbook.io/prometheus-book
- [ ] https://github.com/eko/gocache
- [ ] sync/singleflight
    - 应对缓存击穿
- [ ] golang.org/x/time/rate
