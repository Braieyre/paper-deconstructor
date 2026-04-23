# Paper Deconstructor — First Principles

**知识溯源导师，不是论文摘要机器。**  
A knowledge-tracing mentor for research papers, not a summarization tool.

---

## 这是什么 / What is this?

这是一个 [Claude Code](https://claude.ai/code) Skill，帮助你从**第一性原理**出发，真正读懂一篇研究论文。

它不会给你一份摘要，而是陪你走完一段完整的认知旅程：

1. 建立论文的**知识依赖地图**（知道自己需要什么前置知识）
2. 从论文所在领域**逐层反向溯源**到基础学科
3. 带着这份理解**回归论文**，真正读懂它
4. 通过 Socratic 对话**检验和巩固**理解

---

This is a [Claude Code](https://claude.ai/code) Skill that helps you *truly understand* a research paper from **first principles** — not just read its abstract.

Instead of a summary, it walks you through:

1. Mapping the paper's **knowledge dependencies**
2. **Tracing back** through knowledge layers, from the paper's field to foundational science
3. **Returning to the paper** with a solid foundation to read it deeply
4. A **Socratic dialogue** to validate your understanding

---

## 安装 / Installation

**需要 [Claude Code](https://claude.ai/code)**

### 方法一：复制文件到 Skill 目录

```bash
# macOS / Linux
cp SKILL.md ~/.claude/skills/paper-deconstructor.md
```

> 如果目录不存在，先运行 `mkdir -p ~/.claude/skills`

### 方法二：在 Claude Code 中直接粘贴

打开 Claude Code，运行 `/skills add`，按提示粘贴 `SKILL.md` 的内容。

---

**Requires [Claude Code](https://claude.ai/code)**

### Option 1: Copy to skills directory

```bash
# macOS / Linux
cp SKILL.md ~/.claude/skills/paper-deconstructor.md
```

> Create the directory first if it doesn't exist: `mkdir -p ~/.claude/skills`

### Option 2: Paste directly in Claude Code

Open Claude Code, run `/skills add`, and paste the contents of `SKILL.md` when prompted.

---

## 使用方法 / Usage

安装后，在 Claude Code 中用以下任意方式触发：

| 触发方式 | 示例 |
|---|---|
| 指令（中文） | `帮我拆解这篇论文` / `我想读懂这篇文章` / `从第一性原理理解这篇论文` |
| 指令（英文） | `help me understand this paper from first principles` |
| 斜杠命令 | `/deconstruct` |

支持的输入格式：
- **PDF 文件**：直接上传
- **DOI**：如 `10.1038/s41586-021-03819-2`
- **arXiv 链接**：如 `https://arxiv.org/abs/2303.08774`
- **论文标题 + 作者**

---

After installation, trigger it in Claude Code with any of:

| Trigger | Example |
|---|---|
| Chinese phrase | `帮我拆解这篇论文` / `从第一性原理理解这篇论文` |
| English phrase | `help me understand this paper from first principles` |
| Slash command | `/deconstruct` |

Accepted input formats:
- **PDF file**: upload directly
- **DOI**: e.g. `10.1038/s41586-021-03819-2`
- **arXiv link**: e.g. `https://arxiv.org/abs/2303.08774`
- **Title + author**

---

## 五阶段流程 / Five-Phase Protocol

```
Phase 0  论文解析      →  建立知识依赖地图（Layer 1–4）
Phase 1  逐层溯源      →  从领域知识剥到基础学科（洋葱剥法）
Phase 2  回归论文      →  结构、问题来源、实验设计、结果、贡献与局限
Phase 3  Socratic 收尾 →  3–5 个开放问题，检验真实理解
```

每一步都会**暂停等待你确认**，深度由你控制，不由 AI 单方面决定。

---

## 示例输出 / Example Output

**Phase 0 知识依赖地图（节选）：**

```
论文核心问题：为什么大型语言模型在 few-shot 提示下表现优异？

知识层级结构（从论文到地基）：

Layer 4 ｜ 本论文的核心贡献概念
  └─ In-context learning、Emergent abilities、Scaling laws

Layer 3 ｜ 所属领域的专业知识
  └─ Transformer 架构、Pre-training、Fine-tuning、Prompt engineering

Layer 2 ｜ 支撑该领域的基础学科
  └─ 深度学习（Deep Learning）→ 反向传播、注意力机制
  └─ 统计学习理论（Statistical Learning Theory）→ 泛化界、偏差-方差权衡

Layer 1 ｜ 底层基础学科
  └─ 线性代数、概率论、信息论
```

---

## 贡献 / Contributing

欢迎提 Issue 和 PR，详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## License

MIT © [Braieyre](https://github.com/Braieyre)
