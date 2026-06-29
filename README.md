<div align="center">

# Hi, I'm ShenJun

**Full-Stack Developer | Java Backend | TypeScript | AI Applications**

<sub>湖南 · China · Java 后端 + TypeScript 全栈 · AI 赋能产品交付</sub>

</div>

<img alt="divider" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" />

## About Me

- 全栈开发工程师，主线能力覆盖 `Java/Spring Boot` 后端、`TypeScript` 全栈、桌面端与 AI 应用落地。
- 熟悉企业级 REST API、实时 WebSocket、支付计费、对象存储、缓存与消息队列等业务系统建设。
- 近阶段重点实践 AI 编程工具、LangChain4j、MCP Server、RAG 知识库、实时 ASR 与 AI Agent 任务系统。
- 偏好简单、清晰、可维护的工程实现，关注系统健壮性、商业化闭环和真实业务交付。

## Tech Stack

```text
Languages     Java, TypeScript, JavaScript, Golang, Python, SQL, Rust/C++ basics
Backend       Spring Boot, Spring MVC, Spring Cloud Alibaba, NestJS, MyBatis-Plus, Prisma, Drizzle ORM
Frontend      React 19, Next.js, Zustand, Vue, Electron, Tauri 2.0
AI / RAG      LangChain4j, Spring AI, MCP Server, OpenAI-compatible Gateway, Milvus, SSE, ASR/AST
Database      MySQL, PostgreSQL, Redis, SQLite, InnoDB, index/transaction tuning
Infra         Docker, PM2, Nginx, Linux, RocketMQ, ShardingSphere, Sentinel
Payments      Stripe Connect, WeChat Pay v3, Alipay SDK
Storage       AWS S3, Tencent COS
Tools         Git, Maven, IntelliJ IDEA, VS Code, Postman, Claude Code, Codex
```

## Highlights

- 2023 一带一路暨金砖国家技能发展与技术创新大赛“区块链应用开发与运维”全国一等奖。
- 2023 “中银杯”全国计算机技能大赛 - 区块链技术应用全国二等奖。
- 2025 中国计算机设计大赛“软件应用与开发 - Web 应用与开发”全国三等奖。
- 能从 0 到 1 独立交付产品：桌面端、后端 API、AI 网关、计费系统、支付验签、部署与排查。

## Featured Projects

### LiveQA - AI 实时直播问答助手

`Electron` `React 19` `Zustand` `C++ N-API` `NestJS` `Prisma` `MySQL` `WebSocket` `ASR` `WeChat Pay` `Alipay`

面向直播带货、在线连麦与线下教学场景，提供实时语音转写、弹幕抓取、观众画像、问题提取、术语解析与 AI 回答建议。

- 负责桌面端三进程架构，将音频采集与 ASR 放入独立子进程，降低原生插件异常对主窗口的影响。
- 将 ASR 从客户端直连改为后端网关代理，隐藏火山引擎密钥，并实现 60s 连接上限下的无感轮转。
- 设计后端墙钟滚动扣费，结合 Decimal 高精度与 CAS 游标避免重复扣费和客户端伪造时长。
- 落地 OpenAI 兼容 AI 网关、扫码支付、验签、防重复发放、会员积分与流水聚合。

### Coursedude - AI 课堂学习助手

`Tauri 2.0` `Spring Boot 3.2` `MyBatis-Plus` `MySQL` `Redis` `LangChain4j` `Protobuf` `Stripe` `Tencent COS` `Zustand`

面向海外留学生，解决上课听不懂、笔记记不全、课后难复习等问题，支持实时转写翻译、主题总结、术语解析、AI 问答与 DeepNote 精讲笔记。

- 构建端云协同实时翻译流水线，桌面端 PCM 经后端代理转发火山 AST v2，密钥仅保存在服务端。
- 实现 LIVE 滚动扣、UPLOAD 一次结、崩溃 TIMEOUT 兜底和每日对账的双层计费引擎。
- 设计 Agent 化 DeepNote 生成流程，融合实时转写、精转写和课件文本生成图文笔记。
- 在 Tauri 桌面端落地 Rust 音频采集、SQLite 缓存、弱网重连与后台收尾机制。

### Agenation - 算力与 AI Agent 任务撮合平台

`TypeScript` `NestJS 11` `Next.js 15` `Electron 33` `Drizzle ORM` `PostgreSQL` `WebSocket` `dockerode` `Stripe Connect` `AWS S3` `MCP`

面向分布式闲置算力变现与 AI Agent 任务经济，支持任务发布、Worker 自动接单、本地 Docker 沙盒执行、反作弊校验、积分结算和提现。

- 设计 WebSocket 实时派单，通过加权随机、硬件过滤和原子 CAS 配额校验避免任务超发。
- 实现交易级积分结算，使用成交价快照隔离挂牌价变化，单事务完成反作弊链与原子入账。
- 构建三层孤儿回收机制，应对节点掉线、进程重启和内存定时器丢失。
- 将 Worker 内核从 Electron 解耦，并通过 MCP Server 打通 AI Agent 接单能力。

### Sage RAG - 企业内部知识库问答平台

`Java 17` `Spring Boot 3` `Spring AI` `MyBatis-Plus` `React 18` `Milvus` `Redis` `MySQL` `Sa-Token` `Apache Tika` `SSE`

面向企业内部员工，将流程规范、办公指引、IT 手册、HR 制度和 FAQ 收敛到知识库，提供文档检索与智能问答能力。

- 采用三态熔断器、优先级降级链和流式首包探测保障多模型高可用。
- 基于 SSE 实现问答流式返回，支持前端增量渲染和连接生命周期处理。
- 使用 Apache Tika 完成多格式文档解析，并支持固定大小与结构感知分块。
- 设计会话记忆滑动窗口与摘要写入机制，在控制 Token 成本的同时保留关键上下文。

### LinkCloud - 企业级 SaaS 短链接平台

`Spring Boot` `Spring Cloud Alibaba` `RocketMQ` `ShardingSphere` `Redis` `MySQL` `Sentinel`

面向高并发短链跳转、热点访问和实时数据统计，使用微服务架构支撑低延迟跳转与可扩展的数据分析能力。

- 基于 ShardingSphere 设计短链 Hash 自定义分片算法，支持大规模数据水平扩展。
- 使用 MurmurHash + Base62 生成短链接，并结合布隆过滤器做高性能防重。
- 封装高并发缓存防击穿组件，通过双重检查锁和 Cache-Aside 保证热点数据稳定访问。
- 使用 RocketMQ 异步记录访问日志，支撑访问统计与分析链路。

## GitHub Activity

- 主要活跃方向：`Java/Spring`、`TypeScript/NestJS`、`React/Next.js`、`AI 工程化`、`桌面端产品`。
- 当前主页优先使用文字内容和 GitHub 原生能力，减少第三方统计卡片在不同网络环境下的加载失败。

## Contribution Snake

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ajaxpppp/ajaxpppp/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ajaxpppp/ajaxpppp/output/github-contribution-grid-snake.svg">
    <img alt="GitHub contribution grid snake animation" src="https://raw.githubusercontent.com/ajaxpppp/ajaxpppp/output/github-contribution-grid-snake.svg">
  </picture>
</div>

## Dev Quote

> Talk is cheap. Show me the code.
>
> Linus Torvalds

<div align="center">
  <img alt="divider" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" />
  
  <h3>Let's Connect</h3>
  <p>欢迎通过 <a href="https://github.com/ajaxpppp">GitHub</a> 或 <a href="mailto:18528260613@163.com">Email</a> 与我联系，一起合作项目或交流技术。</p>
  <p>Feel free to reach out via <a href="https://github.com/ajaxpppp">GitHub</a> or <a href="mailto:18528260613@163.com">Email</a> to collaborate or chat about technology.</p>
  
  <sub>From <a href="https://github.com/ajaxpppp">ajaxpppp</a> with care</sub>
</div>
