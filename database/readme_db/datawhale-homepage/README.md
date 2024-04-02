# datawhale 官网项目

## 一、技术选型

- 编程语言：typescript
- 后端框架：express
- 部署工具：pm2

## 二、目录结构

| 文件目录         | 说明       |
| ---------------- | ---------- |
| ./README.md      | 说明文档   |
| ./package        | 源代码     |
| ./package/client | 前端源代码 |
| ./package/server | 后端源代码 |

## 三、开发指南

执行`bootstrap`命令安装 pnpm 和 pm2（如果你没有这两个东西的话）
使用`pnpm install`命令安装依赖
使用`dev:all`命令进行开发，访问`localhost:8081`即可看到网站
使用`build:all`命令进行打包
使用`format`命令格式化代码

## 四、部署指南

执行`bootstrap`命令安装 pnpm 和 pm2（如果你没有这两个东西的话）
使用`start`命令启动服务
