# Hi, I'm Li Jinan

一个正在把项目从本地代码推进到真实线上作品的全栈开发者。

我关注 Java 后端、Vue 前端、AI 应用开发和项目部署。最近完成了一个 AI 零代码应用生成平台的线上部署，从前端静态资源、Nginx 反向代理、后端 Jar 启动，到 MySQL / Redis、接口文档和 AI Key 接入，已经形成可访问、可演示、可继续迭代的完整作品。

## Featured Project

### 今安 AI 应用开发平台

> 用户输入自然语言需求后，系统自动创建应用、调用 AI 生成页面代码，并支持实时预览、源码下载和部署操作。

| 类型 | 地址 |
| --- | --- |
| 在线体验 | [http://124.221.85.117](http://124.221.85.117) |
| 接口文档 | [http://124.221.85.117/api/doc.html#/home](http://124.221.85.117/api/doc.html#/home) |

**核心能力**

- AI 应用生成：根据用户提示词创建应用并生成页面代码
- 实时预览：生成过程和网页效果可在前端页面中查看
- 应用部署：支持下载代码和部署生成后的应用
- 用户体系：支持登录、应用管理、对话记录等基础业务能力
- 接口文档：通过 Knife4j 提供线上接口调试入口

**部署链路**

- 前端：Vue 3 + Vite 构建静态资源，由 Nginx 托管
- 后端：Spring Boot 3 Jar 使用生产环境配置启动
- 代理：Nginx 将 `/api` 请求反向代理到后端服务
- 数据：MySQL 持久化业务数据，Redis 支撑缓存能力
- AI：接入 AI Key，完成应用创建和代码生成链路

## Tech Stack

![Java](https://img.shields.io/badge/Java-17+-orange?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=flat-square)
![Vue](https://img.shields.io/badge/Vue-3-42b883?style=flat-square)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square)

## What I'm Building

- 用 Spring Boot 构建稳定的后端服务
- 用 Vue 3 / TypeScript 打磨前端交互体验
- 把 AI 能力接入真实业务流程
- 学习并实践线上部署、接口文档、缓存、反向代理和生产环境配置

## Project Snapshot

真实截图会继续补充到这里，包括首页、登录成功、创建应用成功、AI 生成页面和生成结果预览。

## GitHub Stats

![Li-Jinan's GitHub stats](https://github-readme-stats.vercel.app/api?username=Li-Jinan&show_icons=true&theme=default&hide_border=true)

