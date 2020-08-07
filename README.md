## 📗 目录结构

```shell
├── api              // api 存放
│   └── v1
├── config           // 常量以及配置结构体
├── core             // 组件模块初始化
├── docs             // swagger 文档
├── env              // 环境配置文件
├── global           // 全局变量
│   └── response
├── initialize       // 组件模块定义
├── log              // 日志存放
├── middleware       // 中间件
├── model            // 结构体存放
│   ├── model_name
│   ├── request
│   └── response
├── router           // 路由层
├── service          // 主要存放mysql 操作文件
├── sql              // 服务mysql 结构存放
└── utils            // 定义的工具方法
```

## 🛠️ 快速开始

直接Clone项目，文件比较全

TIPS: 需要本地安装MySQL数据库和 Redis

```bash
# 下载安装，可以不用是 GOPATH

# 进入到下载目录
cd goApi

# 运行
./admin.sh restart devl 
```


## 💻 常用命令

- ./admin status  查看服务状态
- ./admin start   启动服务
- ./admin build   编译项目
- ./admin restart 重启项目
- ./admin stop    停止项目


## 📝 接口文档
`http://localhost:8900/docs/swagger/index.html`


本项目根据gin_vue_admin开源框架提取后端部分进行二次开发,原文地址: https://github.com/flipped-aurora/gin-vue-admin

数据库相关部分采用原生sql处理，可以使用以下语句生成相关数据库内容 go-mygen -h localhost -P 3306 -u root -p passwd -d dbname