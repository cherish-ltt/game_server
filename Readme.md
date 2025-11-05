# AeroX

AeroX是一款高速、轻量的网络服务器框架，适用于快速构建游戏后端服务器、消息转发等应用。

### 一. 核心架构概述

AeroX采用分层和事件驱动架构，分为三层：

- **网络层（Network Layer）**：基于Reactor模式处理TCP连接和I/O，实现高并发网络处理。
- **逻辑层（Logic Layer）**：基于Actor模型处理业务逻辑，每个用户或实体作为独立actor，避免共享状态竞争。
- **数据层（ECS Layer）**：基于ECS（Entity-Component-System）管理服务器状态。

简易架构图：

```
[客户端] <-> [网络层: Reactor] <-> [逻辑层: Actor系统] <-> [数据层: ECS]
```

### 开源协议

MIT license

### 关于贡献

除非您另有明确说明，否则您有意提交以包含在AeroX中的任何贡献都应被许可为MIT，无需任何额外的条款或条件。
