# GoForum

### 项目介绍：

使用 Go 编写的一个基本功能类似于 Reddit 的论坛。项目采用的前后端分离，采用 RESTful 架构，使用 CLD 分层。

### 我的收获：

- 使用分布式 ID 生成器，雪花算法生成用户 ID
- 利用 Validator 库来校验参数
- 基于 Token 的认证模式
- 限制同一时间只允许一台设备登录
- 使用令牌桶限流,限制到达系统的并发请求数
- 解决代码循环引入问题
- swagger 生成接口文档
- 帖子排名算法
- 优雅关机与重启

### 使用技术：

- 数据库：		MySQL+Redis
- 配置文件管理： Viper
- 日志框架：	Zap
- web 框架：	Gin
- ORM框架：	SqlX

### 项目结构：

- conf:		服务配置
- controller:	控制层
- dao:			数据库层
- docs:		swagger 文件
- logger:		日志库
- logic：		逻辑层
- middlewares：中间件
- models:		模型层
- pkg:			服务共有代码
- router:		路由
- test:			测试
