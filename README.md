# 李今安 | Java 后端与 AI 应用工程

电子科技大学计算机科学与工程学院电子信息专业硕士在读。关注 Java 后端、LLM 应用工程、Tool Calling、Agent 执行链路与微服务系统可靠性与可观测性。

我主要做的是把模型能力接入可运行的业务系统：处理长任务、上下文、工具调用、安全边界、失败恢复与部署问题。

## 技术方向

- Java：Java 21、Spring Boot、Spring Cloud、MySQL、Redis。
- AI 应用：LangChain4j、Spring AI、Tool Calling、MCP、流式输出与上下文管理。
- 系统工程：后台任务、状态持久化、故障恢复、Dubbo、Nacos、Docker Compose、Nginx、Micrometer、Prometheus、Grafana。
- 前端与交付：Vue 3、在线预览、代码下载与应用部署。

## 代表项目

### [今安 AI 应用开发平台](https://github.com/Li-Jinan/code-ai-agent)

[在线体验](https://ai.lijinan.cn) · [接口文档](https://ai.lijinan.cn/api/doc.html#/home)

基于开源项目 [liyupi/yu-ai-code-mother](https://github.com/liyupi/yu-ai-code-mother) 二次开发的 AI 网站生成平台，支持需求输入、代码生成、持续编辑、在线预览、源码下载与部署。

我完成并公开了以下可核验改造：

- 将长耗时生成改为可恢复的后台任务，持久化执行状态并在产物可预览后确认成功：[9a37a62](https://github.com/Li-Jinan/code-ai-agent/commit/9a37a62)、[2c1dbbe](https://github.com/Li-Jinan/code-ai-agent/commit/2c1dbbe)。
- 隔离 Vue 生成会话中的历史工具消息，识别工具调用协议异常：[aa77392](https://github.com/Li-Jinan/code-ai-agent/commit/aa77392)。
- 限制文件工具遍历范围和输出规模，补充路径穿越校验；修复异步回调中的监控上下文传递：[ea5783b](https://github.com/Li-Jinan/code-ai-agent/commit/ea5783b)。
- 完成 MySQL、Redis、Nacos、Selenium 与三个 Dubbo 服务的容器编排、健康检查及统一入口配置：[项目 README](https://github.com/Li-Jinan/code-ai-agent#项目来源与二次开发说明)。
- 心跳过期判断改为与写入同源的数据库时钟，修复数据库与 JVM 时区不一致时任务被误回收的潜伏问题，真实 MySQL 集成测试覆盖 UTC 与 +08:00：[51e5101](https://github.com/Li-Jinan/code-ai-agent/commit/51e5101)。
- 为生成任务补充 Micrometer 指标、Prometheus/Grafana 面板和可复现实验数据：[效果数据](https://github.com/Li-Jinan/code-ai-agent#效果数据)、[PR #2](https://github.com/Li-Jinan/code-ai-agent/pull/2)。

## 其他项目

- [Work App Agent](https://github.com/Li-Jinan/workAppAgent)：基于 [liyupi/yu-ai-agent](https://github.com/liyupi/yu-ai-agent) 的 Spring AI 学习与二次开发项目，个人改动为 Agent 专用线程池、文件工具路径穿越防护与搜索工具边界处理（[2b0df01](https://github.com/Li-Jinan/workAppAgent/commit/2b0df0110409340621e40c6784eefc5271842a71)）。

## 教育背景

- 电子科技大学，计算机科学与工程学院，电子信息硕士，2024.09–2027.06。
- 重庆理工大学，国际学院，计算机科学与技术本科，2019.09–2023.06。

## 联系方式

- Email：1933521002@qq.com
- GitHub：[@Li-Jinan](https://github.com/Li-Jinan)
