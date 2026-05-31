# 李今安 - 腾讯技术开发岗 / Java 后端开发简历文本

## 个人定位

电子科技大学计算机科学与工程学院电子信息专业硕士在读，求职方向为腾讯技术开发岗 / Java 后端开发。具备 Java、Spring Boot、MySQL、Redis、WebSocket、分库分表、权限系统和线上部署实践，能够围绕业务场景完成接口设计、数据建模、缓存优化、并发控制和工程交付。AI Agent、RAG、Tool Calling 和 MCP 为个人加分方向。

## 教育经历

- 电子科技大学，计算机科学与工程学院，电子信息硕士，2024.09 - 2027.06
- 重庆理工大学，国际学院，计算机科学与技术本科，2019.09 - 2023.06

## 专业技能

- Java：掌握集合、异常处理、反射、动态代理等核心机制，理解 HashMap 底层结构和扩容机制。
- 后端框架：熟悉 Spring Boot、MyBatis-Plus，能够使用 Hutool、Lombok 等工具提升工程开发效率。
- 数据库：熟悉 MySQL 表结构设计、索引优化、SQL 调优，实践过 ShardingSphere 动态分表。
- 缓存：熟悉 Redis、Caffeine 多级缓存，实践过 Session 分布式存储、随机过期、缓存雪崩/穿透处理。
- 权限：实践过 Sa-Token、自定义注解、Spring AOP、多账号 RBAC 和方法级鉴权。
- 网络：熟悉 TCP/IP 基础，基于 WebSocket 实践过多人实时协同编辑业务。
- 部署：熟悉 Docker、Nginx、Jar 启动、Serverless 部署和线上接口文档发布。
- AI 应用：熟悉 Spring AI、LangChain4j、RAG、Tool Calling、MCP、Advisor、PgVector 和 Prompt 优化。

## 项目经历

### 领域驱动企业协同云图库

2026.01 - 2026.03

项目简介：基于 Spring Boot + Redis + Caffeine + Sa-Token + ShardingSphere + Disruptor + WebSocket 构建的高并发协作图库系统。系统支持公共图库、私有空间、团队空间、实时协同编辑、图片审核、空间分析、批量管理和 AI 扩图。通过 Redis 分布式状态管理、Sa-Token 细粒度 RBAC、ShardingSphere 动态分片实现多权限用户数据隔离与高效路由；采用 WebSocket + Disruptor 事件驱动模型支撑实时协同编辑。

主要工作：

- 基于 Redis 实现 Session 分布式存储，结合自定义注解 + Spring AOP 统一鉴权框架，支持 5 类操作级权限控制，在多节点部署下实现稳定扩展，鉴权代码重复率降低 60%。
- 构建 Redis + Caffeine 多级缓存体系，引入随机过期时间机制缓解缓存雪崩问题，在热点高并发场景下将缓存命中率提升至 90%+，显著降低数据库压力。
- 封装 COS 通用文件服务，结合图片元信息解析，上传前完成 WebP 转码和缩略图生成，图片体积平均压缩 60%，提升页面加载速度。
- 基于 Sa-Token Kit 模式构建多账号 RBAC 权限模型，通过统一请求上下文与注解合并实现方法级鉴权，权限逻辑复用度提升 70%。
- 采用分段锁 + TransactionTemplate 实现编程式事务，结合限流与预校验机制控制空间容量，在协同与批量场景下使批处理效率提升 3 倍。
- 基于 ShardingSphere 自定义分表算法实现团队图片动态分表，并结合分片节点校验机制保障路由准确性，支持千万级数据规模下的稳定查询。
- 采用 Disruptor 无锁队列对 WebSocket 消息进行异步化处理，引入编辑锁机制避免冲突，系统峰值吞吐能力提升 2 倍，保持毫秒级响应。

项目链接：https://github.com/Li-Jinan/lijinanPicture

### AI Agent 智能体对话应用

2025.10 - 2025.12

项目简介：基于 Spring AI + Spring Boot + RAG + Tool Calling + MCP 构建的多模型 AI 智能体应用。系统支持 ReAct 自主思考、多轮对话隔离、记忆持久化、RAG 知识库检索、结构化输出、Prompt 优化、工具调用和 MCP 服务接入。

主要工作：

- 基于 Spring AI 统一接入灵积与本地部署 Ollama，构建多模型可切换策略，在保证模型能力的同时将 API 调用成本降低 50%。
- 基于 Spring AI ChatMemory + Advisor 实现多轮对话记忆体系，结合 Caffeine 预加载历史会话数据，在高并发场景下将上下文命中率提升至 95%，平均响应延迟降低 30%。
- 构建 MySQL + Redis 分层持久化架构，引入 Kryo 序列化，使序列化体积减少 60%、读写性能提升 2-3 倍，重启后上下文恢复率达 99%。
- 搭建完整 RAG 知识检索体系，完成文档 ETL、PgVector 向量存储、多查询扩展与查询重写，使知识问答准确率提升 45%。
- 集成 6 类工具调用并设计统一注册与调度机制，结合 ToolContext 实现用户身份传递与参数校验，减少无效执行并提升系统稳定性。
- 开发支持 Stdio 与 SSE 双传输模式的 MCP 图片搜索服务并采用 Serverless 部署，降低跨项目接入成本。
- 基于 OpenManus 引入 Human-in-the-Loop 架构，并增加步数限制与死循环检测机制，使系统异常中断率下降。
- 通过 SseEmitter + CompletableFuture 实现流式输出与异步推理架构，实时输出执行过程，降低用户等待感。

项目链接：https://github.com/Li-Jinan/code-ai-agent

## 荣誉奖项

- ACM 校三等奖
- 2021 RoboCup 赛事国二等奖
- 本科与研究生期间多次获得奖学金
- CET-6

## 联系方式

- Email: 1933521002@qq.com
