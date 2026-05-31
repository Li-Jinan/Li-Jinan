# 李今安 | Java 后端 / AI 应用开发

电子科技大学计算机科学与工程学院电子信息专业硕士在读，求职方向为技术开发岗，重点关注 Java 后端开发、高并发服务、缓存与数据库优化、实时协同系统和 AI 应用工程化。

我更希望自己被看作一名后端工程候选人：有 Java / Spring Boot / MySQL / Redis 的基础工程能力，也有把 AI、WebSocket、分库分表、权限系统和部署链路落到真实项目里的实践经验。

## 求职定位

- 目标岗位：腾讯技术开发岗 / Java 后端开发
- 核心能力：Java 后端服务、业务建模、缓存设计、数据库优化、权限系统、WebSocket 实时协同、工程部署
- 加分方向：Spring AI、RAG、Tool Calling、MCP、AI Agent 应用开发

## 教育背景

- 电子科技大学，计算机科学与工程学院，电子信息硕士，2024.09 - 2027.06
- 重庆理工大学，国际学院，计算机科学与技术本科，2019.09 - 2023.06

## 技术能力

- Java 基础：掌握集合、异常处理、反射、动态代理等核心机制，理解 HashMap 底层结构和扩容机制。
- 后端框架：熟悉 Spring Boot、MyBatis-Plus，能够完成接口设计、业务分层、参数校验、异常处理和工程化开发。
- 数据库：熟悉 MySQL 表结构设计、索引优化、SQL 调优和 ShardingSphere 分库分表实践。
- 缓存与性能：熟悉 Redis、Caffeine 多级缓存，实践过随机过期、缓存穿透/雪崩处理和会话分布式存储。
- 权限与安全：实践过 Sa-Token、多账号 RBAC、自定义注解 + AOP 方法级鉴权。
- 网络与协同：熟悉 TCP/IP 基础，基于 WebSocket + Disruptor 实现过多人实时协同编辑。
- 工程部署：熟悉 Docker、Nginx、Jar 进程部署、Serverless 和线上接口文档发布。
- AI 应用：熟悉 Spring AI、LangChain4j、RAG、Tool Calling、MCP、Advisor、PgVector 和 Prompt 优化。

## 重点项目

### 领域驱动企业协同云图库

Repository: [lijinanPicture](https://github.com/Li-Jinan/lijinanPicture)

基于 Spring Boot + Redis + Caffeine + Sa-Token + ShardingSphere + Disruptor + WebSocket 构建的高并发协作图库系统。项目覆盖公共图库、私有空间、团队空间、实时协同编辑、图片审核、空间分析、批量管理和 AI 扩图等业务。

面试官可能关注的后端点：

- 权限体系：基于 Redis Session、自定义注解和 Spring AOP 实现统一鉴权，支持 5 类操作级权限控制，降低鉴权代码重复率。
- 缓存设计：构建 Redis + Caffeine 多级缓存体系，引入随机过期时间缓解缓存雪崩，降低热点查询下的数据库压力。
- 数据规模：基于 ShardingSphere 自定义分表算法实现团队空间图片动态分表，结合分片节点校验保障路由准确性。
- 并发控制：采用分段锁 + TransactionTemplate 控制空间容量和批量编辑事务边界，提升协同和批处理场景稳定性。
- 实时协同：采用 WebSocket + Disruptor 无锁队列异步处理编辑消息，引入编辑锁机制避免冲突，提高峰值吞吐能力。
- 文件服务：封装 COS 通用上传能力，结合图片元信息解析、WebP 转码和缩略图生成优化图片加载体验。

### AI Agent 智能体对话应用

Repository: [code-ai-agent](https://github.com/Li-Jinan/code-ai-agent)

基于 Spring AI + Spring Boot + RAG + Tool Calling + MCP 构建的多模型 AI 智能体应用，支持 ReAct 自主思考、多轮对话隔离、记忆持久化、知识库检索、结构化输出和流式响应。

面试官可能关注的后端点：

- 模型接入：统一接入灵积与本地 Ollama，封装多模型可切换策略，兼顾成本和效果。
- 记忆体系：基于 Spring AI ChatMemory + Advisor 实现多轮对话记忆，结合 Caffeine 预加载历史会话数据。
- 持久化：构建 MySQL + Redis 分层持久化架构，引入 Kryo 序列化优化读写体积和性能。
- RAG 检索：完成文档 ETL、PgVector 向量存储、多查询扩展和查询重写，提高知识问答准确性。
- 工具调用：集成 6 类工具调用并设计统一注册与调度机制，通过 ToolContext 传递用户身份并做参数校验。
- MCP 服务：开发支持 Stdio 与 SSE 双传输模式的 MCP 图片搜索服务，并采用 Serverless 部署。
- 异步响应：通过 SseEmitter + CompletableFuture 实现流式输出与异步推理，降低用户等待感。

## 竞赛与荣誉

- ACM 校三等奖
- 2021 RoboCup 赛事国二等奖
- 本科与研究生期间多次获得奖学金
- CET-6

## 联系方式

- Email: 1933521002@qq.com

## 简历文本版

- [腾讯技术开发岗后端向简历文本](resume/tencent-backend.md)

## GitHub Stats

![Li-Jinan's GitHub stats](https://github-readme-stats.vercel.app/api?username=Li-Jinan&show_icons=true&theme=default&hide_border=true)
