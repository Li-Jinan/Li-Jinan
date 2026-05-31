# Hi, I'm Li Jinan

电子科技大学计算机科学与工程学院电子信息专业硕士在读，求职方向为 Java 后端开发与 AI 应用开发。我关注高并发后端服务、企业级业务系统、AI Agent、RAG、Tool Calling、MCP 和项目上线部署。

## Education

- 电子科技大学，计算机科学与工程学院，电子信息硕士，2024.09 - 2027.06
- 重庆理工大学，国际学院，计算机科学与技术本科，2019.09 - 2023.06

## Skills

- Java 基础：集合、异常处理、反射、动态代理，理解 HashMap 底层实现及扩容机制。
- 后端框架：Spring Boot、MyBatis-Plus、Hutool、Lombok，具备接口开发、业务建模和工程化实践经验。
- 数据库与缓存：MySQL 数据库设计、SQL 调优、索引优化、分库分表、Redis、Caffeine 多级缓存、缓存雪崩/穿透处理。
- 网络与协同：熟悉 TCP/IP 网络模型，基于 WebSocket 实践多人实时协同编辑业务。
- 部署能力：熟悉 Docker 容器化、Nginx 反向代理、Dockerfile 编写和 Serverless 部署。
- AI 应用：Spring AI、LangChain4j、RAG、Tool Calling、MCP、Multi-Agent、Prompt 工程、Advisor、PgVector。

## Featured Projects

### AI Agent 智能体对话应用

基于 Spring AI + Spring Boot + RAG + 工具调用 + MCP 构建的多模型 AI 智能体，支持 ReAct 自主思考、多轮对话隔离、记忆持久化、RAG 知识库检索、结构化输出和 Prompt 优化。

- 统一接入灵积与本地 Ollama，构建多模型可切换策略，将 API 调用成本降低 50%。
- 基于 Spring AI ChatMemory + Advisor 实现多轮对话记忆体系，结合 Caffeine 预加载历史会话数据，使上下文命中率提升至 95%，平均响应延迟降低 30%。
- 构建 MySQL + Redis 分层持久化架构，引入 Kryo 序列化，使序列化体积减少 60%、读写性能提升 2-3 倍。
- 搭建 RAG 知识检索体系，完成文档 ETL、PgVector 向量存储、多查询扩展与查询重写，使知识问答准确率提升 45%。
- 开发支持 Stdio 与 SSE 双传输模式的 MCP 图片搜索服务，并采用 Serverless 部署。
- 通过 SseEmitter + CompletableFuture 实现流式输出与异步推理架构，使用户等待感知时间减少 80%。

Repository: [code-ai-agent](https://github.com/Li-Jinan/code-ai-agent)

### 领域驱动企业协同云图库

基于 Spring Boot + Redis + Caffeine + Sa-Token + Disruptor + WebSocket 构建的高并发协作图库系统。系统通过 Redis 分布式状态管理、Sa-Token 细粒度 RBAC、ShardingSphere 动态分片实现多权限用户数据隔离与高效路由，采用 WebSocket + Disruptor 事件驱动模型支撑实时协同编辑。

- 基于 Redis 实现 Session 分布式存储，结合自定义注解与 Spring AOP 统一鉴权框架，支持 5 类操作级权限控制，鉴权代码重复率降低 60%。
- 构建 Redis + Caffeine 多级缓存体系，引入随机过期时间机制解决缓存雪崩问题，在热点高并发场景下将缓存命中率提升至 90%+。
- 封装 COS 通用文件服务，结合数据万象解析图片元信息，上传前完成 WebP 转码和缩略图生成，图片体积平均压缩 60%。
- 基于 Sa-Token Kit 模式构建多账号 RBAC 权限模型，权限逻辑复用度提升 70%。
- 基于 ShardingSphere 自定义分表算法实现团队图片动态分表，支持千万级数据规模下的稳定查询。
- 采用 Disruptor 无锁队列对 WebSocket 消息进行异步化处理，引入编辑锁机制避免冲突，系统峰值吞吐能力提升 2 倍。

Repository: [lijinanPicture](https://github.com/Li-Jinan/lijinanPicture)

## Honors

- ACM 校三等奖
- 2021 RoboCup 赛事国二等奖
- 本科与研究生期间多次获得奖学金
- CET-6

## Contact

- Email: 1933521002@qq.com

## GitHub Stats

![Li-Jinan's GitHub stats](https://github-readme-stats.vercel.app/api?username=Li-Jinan&show_icons=true&theme=default&hide_border=true)
