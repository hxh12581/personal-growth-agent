# Personal Growth Agent

> 基于多 Agent 协作的个人成长智能系统

## 🎯 核心痛点

个人成长过程中面临 CPTSD（复杂性创伤后应激障碍）、拖延症、过度准备、完美主义等深层心理障碍，以及学习效率低下、目标管理混乱、技能掌握缓慢等实际问题。现有工具多为单一功能（如待办事项、番茄钟），无法提供从问题诊断到解决方案执行的完整闭环。

## 🔄 核心逻辑流程

### 长链推理 (Long-Chain Reasoning)

7 阶段深度分析流程：

1. **现象取证** → 收集客观事实，识别矛盾点
2. **假设生成** → 多维度生成可能原因假设
3. **证据搜集** → 验证与排除假设
4. **深度溯源** → 5Why 追问根本原因
5. **本质建模** → 构建统一解释模型
6. **方法匹配** → 匹配科学方法论
7. **计划执行** → 拆解目标，追踪执行

### 多 Agent 协作

5 个专业 Agent 协同工作：

| Agent | 职责 | 核心能力 |
|-------|------|----------|
| DeepTrace | 深度溯源 | 六步本质挖掘、根因分析、矛盾论应用 |
| KnowledgeClassroom | 知识课堂 | 微课堂讲解、方法论匹配、学习路径规划 |
| MicroProgress | 微进度加速 | 智能目标拆解、最小行动设计、个性化计划 |
| ActionTracking | 行动追踪 | 游戏化任务管理、即时反馈、进度可视化 |
| ContentAtomization | 内容原子化 | 日记结构化、标签系统、知识库构建 |

## 🏗️ 快速架构图

```
用户输入
    │
    ▼
┌─────────────────┐
│  Router Agent   │  ← 分析意图，决定 Agent 链
└────────┬────────┘
         │
    ┌────┴────┬────────┬────────┐
    ▼         ▼        ▼        ▼
┌───────┐ ┌───────┐ ┌───────┐ ┌───────┐
│Trace  │ │Knowledge│ │Progress│ │Action │
│溯源   │ │课堂    │ │加速   │ │追踪   │
└───┬───┘ └───────┘ └───┬───┘ └───┬───┘
    │                   │         │
    └───────────────────┴─────────┘
                    │
                    ▼
            ┌───────────────┐
            │  Atomization  │
            │   内容原子化   │
            └───────────────┘
                    │
                    ▼
                用户输出
```

## 📂 项目结构

```
personal-growth-agent/
├── README.md              # 项目说明
├── docs/
│   └── DESIGN.md          # 详细设计文档
├── src/
│   ├── core/              # 核心引擎
│   │   ├── long_chain.py  # 长链推理引擎
│   │   ├── orchestrator.py # 多 Agent 编排器
│   │   └── router.py      # Agent 路由器
│   └── agents/            # Agent 实现
│       ├── deep_trace.py
│       ├── knowledge_classroom.py
│       ├── micro_progress.py
│       ├── action_tracking.py
│       └── content_atomization.py
└── examples/              # 使用示例
```

## 🚀 使用示例

### 示例 1: 解决拖延问题

```
用户: "我总是拖延重要的工作，明明知道应该做，但就是开始不了"

系统分析:
1. DeepTrace → 识别为 CPTSD 导致的"冻结"反应
2. Knowledge → 匹配 CBT 认知重构 + 自我同情方法
3. MicroProgress → 拆解为"5秒法则"最小行动
4. ActionTracking → 设置每日打卡追踪
5. Atomization → 结构化记录每次突破

输出: 完整的疗愈方案 + 可执行的行动计划
```

### 示例 2: 考研复习规划

```
用户: "我想3个月掌握408考研，如何高效复习？"

系统分析:
1. Knowledge → 考频分析 + 方法论匹配（间隔重复、主动回忆）
2. MicroProgress → 智能拆解3个月目标为周/日计划
3. ActionTracking → 刷题追踪 + 游戏化成就系统
4. Atomization → 错题原子化 + 标签管理

输出: 个性化学习计划 + 进度追踪系统
```

## 🛠️ 技术栈

- **核心**: Python 3.10+
- **AI/LLM**: OpenAI API / Claude API
- **Agent框架**: 自研 Multi-Agent Orchestrator
- **数据存储**: Redis (上下文) / PostgreSQL (用户数据)
- **API**: FastAPI

## 📝 核心创新点

1. **方法论融合**: 首次将 CBT、福格模型、刻意练习、毛选方法论系统整合到 AI Agent
2. **长链推理**: 7 阶段深度分析，远超常规对话式 AI 的浅层响应
3. **多 Agent 协作**: 5 个专业 Agent 动态协作，覆盖诊断到执行全流程
4. **闭环设计**: 现象→本质→方法→行动→复盘的完整闭环

## 📄 License

MIT License

## 🤝 Contributing

欢迎提交 Issue 和 PR！

---

**项目状态**: 设计阶段 | **目标**: xiaomi mimo token 申请
