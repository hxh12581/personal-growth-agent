# Personal Growth Agent (PGA)

一个基于多 Agent 协作的个人成长智能系统，通过现象分析、本质挖掘、科学方法匹配、行动执行闭环，帮助用户高效解决 CPTSD、拖延、过度准备等成长障碍，实现快速学习与能力提升。

## 🎯 项目概述

Personal Growth Agent 是一个 AI 驱动的个人成长助手，它不仅仅是简单的任务管理工具，而是一个能够理解用户深层问题、分析根本原因、提供科学解决方案的完整成长生态系统。

### 核心痛点解决

1. **CPTSD 与心理创伤**：通过深度溯源分析，识别并疗愈深层心理模式
2. **拖延与行动 paralysis**：小步快跑进步器拆解目标，最小阻力启动
3. **过度准备与完美主义**：现象-本质-行动闭环，破除无效准备循环
4. **学习效率低下**：知识微课堂 + 智能学习计划匹配，加速技能掌握
5. **目标管理混乱**：内容原子化 + 动态目标拆解，建立清晰成长路径

## 🏗️ 系统架构

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                           Personal Growth Agent                              │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│  ┌─────────────────────────────────────────────────────────────────────┐   │
│  │                        Multi-Agent Orchestrator                      │   │
│  │                     (长链推理调度中心)                                │   │
│  └─────────────────────────────────────────────────────────────────────┘   │
│                                    │                                        │
│           ┌────────────────────────┼────────────────────────┐               │
│           │                        │                        │               │
│           ▼                        ▼                        ▼               │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐             │
│  │  Deep Trace     │  │  Knowledge      │  │  Micro Progress │             │
│  │  Explorer       │  │  Classroom      │  │  Accelerator    │             │
│  │                 │  │                 │  │                 │             │
│  │ • 六步本质挖掘   │  │ • 微课堂讲解    │  │ • 目标拆解      │             │
│  │ • 根因分析       │  │ • 知识点解析    │  │ • 最小行动设计  │             │
│  │ • 矛盾论应用     │  │ • 方法论传授    │  │ • 进度追踪      │             │
│  └────────┬────────┘  └────────┬────────┘  └────────┬────────┘             │
│           │                    │                    │                       │
│           └────────────────────┼────────────────────┘                       │
│                                ▼                                            │
│  ┌─────────────────────────────────────────────────────────────────────┐   │
│  │                     Content Atomization Engine                       │   │
│  │                    (内容原子化与标签系统)                             │   │
│  └─────────────────────────────────────────────────────────────────────┘   │
│                                │                                            │
│                                ▼                                            │
│  ┌─────────────────────────────────────────────────────────────────────┐   │
│  │                     Action Tracking System                           │   │
│  │                    (游戏化行动追踪与反馈)                             │   │
│  └─────────────────────────────────────────────────────────────────────┘   │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

## 🔄 核心逻辑流程

### 长链推理流程 (Long-Chain Reasoning)

```
用户输入问题/目标
    │
    ▼
┌──────────────────────────────────────────────────────────────┐
│ Phase 1: 现象取证 (Phenomenon Documentation)                  │
│ • 收集用户描述的事实                                          │
│ • 识别矛盾点和异常现象                                         │
│ • 输出：现象清单 + 矛盾点                                      │
└──────────────────────────────────────────────────────────────┘
    │
    ▼
┌──────────────────────────────────────────────────────────────┐
│ Phase 2: 深度溯源 (Root Cause Analysis)                       │
│ • 5Why 追问根本原因                                           │
│ • 系统动力学分析                                               │
│ • 输出：根因分析树                                             │
└──────────────────────────────────────────────────────────────┘
    │
    ▼
┌──────────────────────────────────────────────────────────────┐
│ Phase 3: 本质建模 (Essence Modeling)                          │
│ • 构建统一解释框架                                             │
│ • 一句话概括本质                                               │
│ • 输出：本质模型 + 可验证预测                                   │
└──────────────────────────────────────────────────────────────┘
    │
    ▼
┌──────────────────────────────────────────────────────────────┐
│ Phase 4: 方法匹配 (Method Matching)                           │
│ • 根据本质匹配科学方法论                                       │
│ • 知识微课堂讲解相关概念                                       │
│ • 输出：方法论推荐                                             │
└──────────────────────────────────────────────────────────────┘
    │
    ▼
┌──────────────────────────────────────────────────────────────┐
│ Phase 5: 目标拆解 (Goal Decomposition)                        │
│ • 微进度加速器拆解目标                                         │
│ • 设计最小行动单元                                             │
│ • 输出：行动计划                                               │
└──────────────────────────────────────────────────────────────┘
    │
    ▼
┌──────────────────────────────────────────────────────────────┐
│ Phase 6: 执行追踪 (Execution Tracking)                        │
│ • 游戏化任务追踪                                               │
│ • 即时反馈与正强化                                             │
│ • 输出：进度报告 + 调整建议                                     │
└──────────────────────────────────────────────────────────────┘
    │
    ▼
┌──────────────────────────────────────────────────────────────┐
│ Phase 7: 复盘迭代 (Review & Iterate)                          │
│ • 内容原子化整理日记/反思                                      │
│ • 复盘效果，更新模型                                           │
│ • 输出：迭代后的成长档案                                       │
└──────────────────────────────────────────────────────────────┘
```

### 多 Agent 协作机制

```
┌─────────────────────────────────────────────────────────────────┐
│                     User Query                                   │
└─────────────────────────────────────────────────────────────────┘
    │
    ▼
┌─────────────────────────────────────────────────────────────────┐
│              Router Agent (问题路由)                             │
│  • 分析问题类型：心理/学习/行动/知识                            │
│  • 决定 Agent 调用顺序                                          │
└─────────────────────────────────────────────────────────────────┘
    │
    ├─── 心理/行为问题 ───┐
    │                     ▼
    │    ┌─────────────────────────────────────┐
    │    │  Deep Trace Explorer Agent          │
    │    │  • 六步本质挖掘                      │
    │    │  • 根因分析                          │
    │    │  • CPTSD/拖延/完美主义诊断           │
    │    └─────────────────────────────────────┘
    │                     │
    │                     ▼
    │    ┌─────────────────────────────────────┐
    │    │  Knowledge Classroom Agent          │
    │    │  • 匹配心理学/行为科学方法论         │
    │    │  • 微课堂讲解应对策略                │
    │    └─────────────────────────────────────┘
    │
    ├─── 学习目标 ───┐
    │                ▼
    │    ┌─────────────────────────────────────┐
    │    │  Knowledge Classroom Agent          │
    │    │  • 知识点解析                        │
    │    │  • 学习路径规划                      │
    │    └─────────────────────────────────────┘
    │                │
    │                ▼
    │    ┌─────────────────────────────────────┐
    │    │  Micro Progress Accelerator Agent   │
    │    │  • 智能目标拆解                      │
    │    │  • 个性化学习计划                    │
    │    └─────────────────────────────────────┘
    │
    └─── 执行追踪 ───┐
                     ▼
    ┌─────────────────────────────────────┐
    │  Action Tracking Agent              │
    │  • 游戏化任务管理                    │
    │  • 即时反馈系统                      │
    │  • 进度可视化                        │
    └─────────────────────────────────────┘
                     │
                     ▼
    ┌─────────────────────────────────────┐
    │  Content Atomization Agent          │
    │  • 日记/反思结构化                   │
    │  • 标签系统管理                      │
    │  • 知识库构建                        │
    └─────────────────────────────────────┘
```

## 🧩 Agent 详细设计

### 1. Deep Trace Explorer Agent

**职责**：深度溯源分析，挖掘问题本质

**核心能力**：
- 六步本质挖掘法（现象→假设→验证→根因→模型→检验）
- 融合毛选矛盾论与实践论
- 第一性原理分析
- 5Why 根因分析
- 系统动力学建模

**应用场景**：
- CPTSD 创伤模式识别
- 拖延行为深层原因分析
- 完美主义心理机制解析
- 人际关系冲突本质挖掘

### 2. Knowledge Classroom Agent

**职责**：知识传授与方法论匹配

**核心能力**：
- 微课堂形式讲解知识点
- 心理学/行为科学方法论库
- 学习路径智能规划
- 知识点关联推荐

**应用场景**：
- CBT 认知行为疗法教学
- 福格行为模型讲解
- 刻意练习方法传授
- 时间管理技巧教学

### 3. Micro Progress Accelerator Agent

**职责**：目标拆解与行动计划设计

**核心能力**：
- 智能目标层级拆解（年→月→周→日→最小行动）
- 最小阻力原则应用
- 触发器设计
- 个性化学习计划匹配

**应用场景**：
- 考研复习计划制定
- 技能学习路径规划
- 习惯养成计划设计
- 项目目标拆解

### 4. Action Tracking Agent

**职责**：游戏化行动追踪与反馈

**核心能力**：
- 任务进度追踪
- 游戏化奖励机制
- 即时反馈系统
- 数据可视化

**应用场景**：
- 每日任务打卡
- 学习进度追踪
- 习惯养成记录
- 成就系统管理

### 5. Content Atomization Agent

**职责**：内容结构化与知识管理

**核心能力**：
- 日记/反思原子化拆分
- 四维度标签系统（主题/类型/作用/情感）
- 知识库构建
- 内容组合推荐

**应用场景**：
- 学习笔记整理
- 日记结构化存储
- 文章素材库构建
- 知识复盘总结

## 📊 技术实现

### 长链推理实现

```python
class LongChainReasoning:
    """长链推理引擎"""
    
    def __init__(self):
        self.agents = {
            'trace': DeepTraceExplorer(),
            'classroom': KnowledgeClassroom(),
            'progress': MicroProgressAccelerator(),
            'action': ActionTracking(),
            'atomization': ContentAtomization()
        }
    
    async def execute(self, query: str, context: dict) -> dict:
        """执行完整推理链"""
        
        # Phase 1: 现象取证
        phenomena = await self.agents['trace'].document_phenomena(query)
        
        # Phase 2: 深度溯源
        root_causes = await self.agents['trace'].analyze_root_cause(phenomena)
        
        # Phase 3: 本质建模
        essence_model = await self.agents['trace'].build_essence_model(root_causes)
        
        # Phase 4: 方法匹配
        methods = await self.agents['classroom'].match_methods(essence_model)
        
        # Phase 5: 目标拆解
        plan = await self.agents['progress'].decompose_goals(methods, context)
        
        # Phase 6: 执行追踪
        tracking = await self.agents['action'].setup_tracking(plan)
        
        # Phase 7: 复盘迭代
        review = await self.agents['atomization'].structure_content(tracking)
        
        return {
            'phenomena': phenomena,
            'root_causes': root_causes,
            'essence_model': essence_model,
            'methods': methods,
            'plan': plan,
            'tracking': tracking,
            'review': review
        }
```

### 多 Agent 协作实现

```python
class MultiAgentOrchestrator:
    """多 Agent 协作编排器"""
    
    async def route_and_execute(self, query: str) -> dict:
        """路由并执行多 Agent 协作"""
        
        # 分析问题类型
        query_type = self.classify_query(query)
        
        # 根据类型构建 Agent 执行链
        if query_type == 'psychological':
            chain = ['trace', 'classroom', 'progress', 'action']
        elif query_type == 'learning':
            chain = ['classroom', 'progress', 'action']
        elif query_type == 'action':
            chain = ['progress', 'action']
        else:
            chain = ['trace', 'classroom', 'progress', 'action', 'atomization']
        
        # 顺序执行 Agent 链
        results = {}
        context = {'query': query}
        
        for agent_name in chain:
            agent = self.agents[agent_name]
            result = await agent.execute(context)
            results[agent_name] = result
            context.update(result)
        
        return results
```

## 🎮 使用示例

### 示例 1: 解决拖延问题

**用户输入**："我总是拖延重要的工作，明明知道应该做，但就是开始不了"

**系统处理流程**：

1. **Deep Trace Explorer** 分析：
   - 现象：任务启动困难、明知重要却不行动
   - 根因：可能涉及完美主义恐惧、任务模糊导致的认知负荷、缺乏即时反馈
   - 本质：高阻力启动 + 恐惧失败的心理机制

2. **Knowledge Classroom** 匹配方法：
   - 讲解"最小阻力原则"
   - 介绍"2分钟法则"
   - 传授"任务拆解"技巧

3. **Micro Progress Accelerator** 制定计划：
   - 将"完成报告"拆解为"打开文档→写标题→写第一段→..."
   - 每个步骤控制在 2-5 分钟
   - 设计触发器："坐到书桌前→立即打开文档"

4. **Action Tracking** 追踪执行：
   - 每日打卡任务
   - 游戏化进度条
   - 连续打卡奖励

5. **Content Atomization** 整理反思：
   - 原子化记录每日执行感受
   - 标签：#拖延 #行动 #心理
   - 积累个人成长档案

### 示例 2: 考研复习规划

**用户输入**："我想3个月掌握408考研，但不知道如何安排"

**系统处理流程**：

1. **Knowledge Classroom** 分析考频：
   - 展示408各科目考频分析
   - 识别高频考点

2. **Micro Progress Accelerator** 拆解目标：
   - 3个月→12周→每周目标
   - 每天2-3小时学习安排
   - 知识点优先级排序

3. **Action Tracking** 追踪进度：
   - 每日刷题记录
   - 正确率统计
   - 薄弱点标记

4. **Content Atomization** 整理错题：
   - 错题原子化存储
   - 标签：#数据结构 #算法 #错题
   - 定期复盘推荐

## 🚀 快速开始

### 安装

```bash
# 克隆项目
git clone https://github.com/hxh12581/personal-growth-agent.git
cd personal-growth-agent

# 安装依赖
pip install -r requirements.txt

# 配置环境变量
cp .env.example .env
# 编辑 .env 文件，添加 API 密钥
```

### 运行

```bash
# 启动完整系统
python -m pga serve

# 或运行单个 Agent
python -m pga.agents.deep_trace
python -m pga.agents.knowledge_classroom
python -m pga.agents.micro_progress
python -m pga.agents.action_tracking
python -m pga.agents.content_atomization
```

## 📁 项目结构

```
personal-growth-agent/
├── docs/                       # 文档
│   ├── architecture.md         # 架构设计
│   ├── agents/                 # Agent 详细文档
│   └── api/                    # API 文档
├── src/                        # 源代码
│   ├── core/                   # 核心引擎
│   │   ├── long_chain.py       # 长链推理引擎
│   │   ├── orchestrator.py     # 多 Agent 编排器
│   │   └── router.py           # 问题路由
│   ├── agents/                 # Agent 实现
│   │   ├── deep_trace.py       # 深度溯源 Agent
│   │   ├── knowledge_classroom.py
│   │   ├── micro_progress.py
│   │   ├── action_tracking.py
│   │   └── content_atomization.py
│   ├── utils/                  # 工具函数
│   └── models/                 # 数据模型
├── examples/                   # 使用示例
├── tests/                      # 测试
├── README.md
├── requirements.txt
└── setup.py
```

## 📝 License

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🤝 Contributing

欢迎提交 Issue 和 PR！详见 [CONTRIBUTING.md](CONTRIBUTING.md)

## 🙏 Acknowledgments

- 方法论基于 CBT 认知行为疗法、福格行为模型、刻意练习等科学理论
- 架构设计参考 ReAct、Reflexion 等 Agent 协作框架
