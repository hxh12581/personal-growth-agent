# Contributing to Personal Growth Agent

感谢您对 Personal Growth Agent 项目的关注！我们欢迎各种形式的贡献。

## 如何贡献

### 报告问题

如果您发现了 bug 或有功能建议，请通过 GitHub Issues 提交：

1. 检查是否已有类似 issue
2. 使用对应的 issue 模板
3. 提供尽可能详细的信息：
   - 问题描述
   - 复现步骤
   - 期望行为
   - 实际行为
   - 环境信息（Python版本、操作系统等）

### 提交代码

1. **Fork 仓库**
   ```bash
   git clone https://github.com/yourusername/personal-growth-agent.git
   cd personal-growth-agent
   ```

2. **创建分支**
   ```bash
   git checkout -b feature/your-feature-name
   # 或
   git checkout -b fix/your-bug-fix
   ```

3. **安装开发依赖**
   ```bash
   pip install -r requirements.txt
   pip install -e ".[dev]"
   ```

4. **编写代码**
   - 遵循 PEP 8 代码风格
   - 添加必要的注释和文档
   - 编写测试用例

5. **运行测试**
   ```bash
   pytest tests/
   ```

6. **提交更改**
   ```bash
   git add .
   git commit -m "feat: add your feature description"
   git push origin feature/your-feature-name
   ```

7. **创建 Pull Request**
   - 提供清晰的 PR 描述
   - 关联相关的 issue
   - 确保 CI 检查通过

## 代码规范

### Python 代码风格

- 遵循 [PEP 8](https://www.python.org/dev/peps/pep-0008/)
- 使用 [Black](https://github.com/psf/black) 格式化代码
- 最大行长度：100 字符

```bash
# 格式化代码
black src/ tests/

# 检查类型
mypy src/
```

### 提交信息规范

使用 [Conventional Commits](https://www.conventionalcommits.org/) 格式：

- `feat:` 新功能
- `fix:` 修复 bug
- `docs:` 文档更新
- `style:` 代码格式（不影响代码运行的变动）
- `refactor:` 重构
- `test:` 测试相关
- `chore:` 构建过程或辅助工具的变动

示例：
```
feat: add new agent for emotional support

- Implement EmotionSupportAgent class
- Add emotion recognition module
- Update orchestrator to route emotional queries
```

### 文档规范

- 所有公共 API 必须包含 docstring
- 使用 Google Style docstring 格式
- 更新 README.md 和 docs/ 下的相关文档

```python
def example_function(param1: str, param2: int) -> bool:
    """
    简要描述函数功能。
    
    详细描述，可以包含多行。
    
    Args:
        param1: 第一个参数的描述
        param2: 第二个参数的描述
        
    Returns:
        返回值的描述
        
    Raises:
        ValueError: 当参数无效时抛出
        
    Example:
        >>> example_function("test", 42)
        True
    """
    pass
```

## 项目结构

```
personal-growth-agent/
├── src/                    # 源代码
│   ├── core/              # 核心引擎
│   ├── agents/            # Agent 实现
│   └── utils/             # 工具函数
├── tests/                 # 测试代码
├── docs/                  # 文档
├── examples/              # 使用示例
└── README.md             # 项目说明
```

## Agent 开发指南

如果您想添加新的 Agent：

1. 继承 `BaseAgent` 类
2. 实现 `execute` 方法
3. 添加单元测试
4. 更新文档

示例：

```python
from src.core.engine import BaseAgent, AgentInput, AgentOutput

class MyNewAgent(BaseAgent):
    async def execute(self, input_data: AgentInput) -> AgentOutput:
        # 实现 Agent 逻辑
        result = await self._process(input_data)
        
        return AgentOutput(
            result=result,
            confidence=0.9,
            next_agent=None,
            metadata={'agent': 'my_new_agent'}
        )
    
    async def validate(self, input_data: AgentInput) -> bool:
        # 验证输入
        return True
```

## 测试指南

### 运行测试

```bash
# 运行所有测试
pytest

# 运行特定测试文件
pytest tests/test_engine.py

# 运行特定测试函数
pytest tests/test_engine.py::test_long_chain_reasoning

# 显示测试覆盖率
pytest --cov=src --cov-report=html
```

### 编写测试

```python
import pytest
from src.core.engine import LongChainReasoning

@pytest.mark.asyncio
async def test_long_chain_reasoning():
    engine = LongChainReasoning()
    
    query = "测试查询"
    user_profile = {'name': '测试用户'}
    
    results = await engine.execute_full_chain(query, user_profile)
    
    assert 'phenomenon' in results
    assert 'essence' in results
    assert 'plan' in results
```

## 发布流程

1. 更新版本号（`setup.py`）
2. 更新 CHANGELOG.md
3. 创建 Git tag
4. 发布到 PyPI

```bash
# 构建发布包
python setup.py sdist bdist_wheel

# 上传到 PyPI
twine upload dist/*
```

## 社区

- GitHub Discussions: 讨论新功能和想法
- GitHub Issues: 报告 bug 和请求功能
- Pull Requests: 提交代码贡献

## 许可证

通过提交代码，您同意您的贡献将在 MIT 许可证下发布。

## 联系我们

如有问题，请通过 GitHub Issues 联系我们。

感谢您的贡献！🦐
