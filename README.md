# 李今安 | AI 应用工程 / Agent Engineering

电子科技大学计算机科学与工程学院电子信息专业硕士在读，方向聚焦 **LLM 应用系统、AI Agent、RAG、Tool Calling、自动化工作流与后端系统集成**。

我更希望自己被看作一名 AI 应用工程候选人：后端服务开发是工程底座，重点能力放在把 LLM、Agent 工作流、工具调用、SSE 流式反馈、微服务治理与对象存储能力落到可运行的业务系统中。

## 求职定位

- 目标方向：AI 应用开发 / Agent 工程 / LLM 应用后端
- 关注领域：Agent 工作流、RAG、Tool Calling、评测与日志追踪、系统集成、自动化工具
- 工程基础：后端接口、前后端联调、对象存储、任务调度、流式响应、部署与接口文档

## 教育背景

- 电子科技大学，计算机科学与工程学院，电子信息硕士，2024.09 - 2027.06
- 重庆理工大学，国际学院，计算机科学与技术本科，2019.09 - 2023.06

## 技术关注

- LLM 应用链路：Prompt 设计、结构化输出、函数/工具调用、上下文管理、流式响应。
- Agent 工程：工具注册、文件操作、任务执行、流程编排、失败退出、执行过程可视化。
- RAG 基础：文档切分、Embedding、向量召回、查询改写、重排、上下文拼接和幻觉控制。
- 平台工程：MinIO/OSS、XXL-JOB、Nginx、任务状态同步、对象存储路径管理、自动化验证。
- 后端基础：业务接口开发、参数校验、异常处理、接口文档维护、MySQL/Redis 常见使用场景。

## 重点项目

### 今安 AI 应用开发平台（code-ai-agent）

Repository: [code-ai-agent](https://github.com/Li-Jinan/code-ai-agent)  
Online: [https://ai.lijinan.cn](https://ai.lijinan.cn)  
API Docs: [https://ai.lijinan.cn/api/doc.html#/home](https://ai.lijinan.cn/api/doc.html#/home)

基于 Vue 3、Spring Boot、LangChain4j、Dubbo 与 Nacos 构建的微服务化 AI 代码生成平台。用户可以通过自然语言生成 HTML、多文件网站或 Vue 项目，并继续完成可视化修改、在线预览、源码下载与部署发布。

重点能力：

- 将应用管理与 AI 生成、用户管理、网页截图拆分为 `app`、`user`、`screenshot` 三个独立服务，通过 Nacos 完成服务注册与发现，并使用 Dubbo 进行内部 RPC 调用。
- 基于 LangChain4j 构建 AI 代码生成服务，支持 HTML、多文件网站和 Vue 项目等生成模式。
- 基于 Tool Calling 封装文件读取、写入、修改、删除和目录读取等工具，使生成项目能够持续迭代。
- 通过 SSE 实时返回模型输出和工具执行信息，前端同步展示生成过程与结果。
- 使用 Redis ChatMemory 隔离应用级对话上下文，并结合 MySQL 对话历史恢复会话；使用 Caffeine 缓存 AI 服务实例、Redisson 实现用户级限流。
- 支持可视化选区修改、iframe 在线预览、源码下载和站点部署；截图服务使用 Selenium 生成作品封面并上传腾讯云 COS。

### Kosmo 激光雷达算法云平台实习

Company: 上海禾赛科技有限公司

参与 Kosmo 云平台中激光雷达 Mesh 算法任务调度与自动化验证相关工作，重点围绕 GPU 算法任务调度、MinIO/OSS 结果同步、自动化 Skill 和第三方平台接入链路展开。

关注能力：

- 算法任务从用户提交、任务入队、GPU 执行到结果回传的异步处理链路。
- 基于 MinIO/OSS `result.json` 的任务状态同步、失败识别和重建流程验证。
- 面向调度场景的自动化 Skill，支持 Mock 算法结果并缩短联调验证时间。
- 第三方平台调用 Kosmo 重建算力与计费能力的接口链路和自动化框架建设。

### Agent 实验项目

- [workAppAgent](https://github.com/Li-Jinan/workAppAgent)：Spring AI / MCP / RAG / Tool Calling 学习与实验项目，面向工作助手与工具调用场景。

## 竞赛与荣誉

- ACM 校三等奖
- 2021 RoboCup 赛事国二等奖
- 本科与研究生期间多次获得奖学金
- CET-6

## 联系方式

- Email: 1933521002@qq.com
- GitHub: [Li-Jinan](https://github.com/Li-Jinan)

## GitHub Stats

![Li-Jinan's GitHub stats](https://github-readme-stats.vercel.app/api?username=Li-Jinan&show_icons=true&theme=default&hide_border=true)
