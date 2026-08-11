# AI修仙人生重来模拟器

一个由 `Spring Boot + FastAPI + Vue 3` 组成的三端协作项目：

- `backend/`：负责人生状态、事件抽签、状态机切换与存档
- `ai-service/`：负责根据上下文生成剧情文本与墓志铭
- `frontend/`：负责属性展示、交互与沉浸式表现
- `shared/`：放置 Java 与 Python 之间的通信协议

## 目录结构

```text
.
├─ backend
├─ ai-service
├─ frontend
├─ shared
└─ docs
```

## 当前阶段

当前仓库已完成第一个可扩展骨架：

- 定义了 Java -> Python 的叙事协议
- 落好了 Spring Boot 后端基础结构
- 落好了 FastAPI AI 服务基础接口
- 落好了 Vue 3 + Pinia 前端基础页面
- 给出了后续 5 周开发蓝图与落地拆分

## 主流程

1. 前端点击“下一岁”
2. 后端推进年龄、抽取事件、计算属性变化
3. 后端调用 AI 服务生成叙事
4. 后端返回最新人生状态
5. 前端展示属性与故事文本

## 后续建议

优先把第 2 周的凡人事件库补全，再进入修仙分支。
