# 示例会话 / Sample Session

本示例展示使用 arXiv 链接触发 Skill 后，Phase 0 知识依赖地图的输出，以及一次知识盲点协议的触发过程。

> **论文：** "Attention Is All You Need" (Vaswani et al., 2017)  
> **链接：** https://arxiv.org/abs/1706.03762

---

## 触发 / Trigger

**用户：**
```
帮我拆解这篇论文：https://arxiv.org/abs/1706.03762
```

**Skill：**
```
你好，把论文给我——PDF、DOI、arXiv 链接或者标题都可以。
我们从第一性原理开始，一层一层把它拆开，再重新读懂它。
```

---

## Phase 0：知识依赖地图

**Skill：**

```
论文核心问题：能否完全抛弃循环结构（RNN）和卷积结构（CNN），
              仅用注意力机制（Attention）来完成序列到序列的建模任务？

知识层级结构（从论文到地基）：

Layer 4 ｜ 本论文的核心贡献概念
  └─ Multi-Head Self-Attention、Positional Encoding、
     Scaled Dot-Product Attention、Encoder-Decoder 架构

Layer 3 ｜ 所属领域的专业知识
  └─ 序列到序列模型（Seq2Seq）、注意力机制（Attention Mechanism）、
     机器翻译（Machine Translation）、语言模型（Language Model）

Layer 2 ｜ 支撑该领域的基础学科
  └─ 深度学习（Deep Learning）→ 反向传播（Backpropagation）、梯度消失问题
  └─ 自然语言处理（NLP）→ 词嵌入（Word Embedding）、词表（Vocabulary）

Layer 1 ｜ 底层基础学科
  └─ 线性代数 → 矩阵乘法、点积（Dot Product）
  └─ 概率论 → Softmax 函数、概率分布
  └─ 信息论 → 交叉熵损失（Cross-Entropy Loss）
```

> 这张地图看起来准确吗？有没有你特别想深挖的方向？  
> 确认后我们从 Layer 3 开始往下剥第一层。

---

**用户：**
```
准确，开始吧。不过 Positional Encoding 是什么我不太清楚。
```

---

## 知识盲点协议触发 / Blind-Spot Protocol

**Skill：**

```
📌 概念速览
Positional Encoding（位置编码）是 Transformer 用来告诉模型"这个词在句子里排第几"的方式。
因为 Self-Attention 本身不区分顺序（它同时看所有词），所以需要手动注入位置信息。
就像在一排无编号的座位上，给每个座位贴上"第1排第3座"的标签。

🔍 想深入学习这个概念：

搜索关键词（中文）：位置编码、Transformer 位置信息
搜索关键词（英文）：positional encoding, transformer position embedding

推荐学习渠道：
• YouTube：搜索 "positional encoding explained" 或 "transformer positional encoding intuition"
• B站：搜索 "Transformer 位置编码 讲解"
• 3Blue1Brown：搜索频道内 "Attention" 系列视频（有极佳的可视化）

可直接复制使用的搜索词：
"YouTube 搜：positional encoding transformer explained，找时长10~20分钟、播放量最高的视频"
```

> 这个解释清楚了吗？我们继续当前这一层吗？

---

**用户：**
```
清楚了，继续。
```

> *(Phase 1 正式开始，从 Layer 3 逐层溯源……)*

---

*完整会话通常包含 Phase 1 → Phase 2 → Phase 3 Socratic 收尾，视论文复杂度和用户节奏，全程约 30–90 分钟。*
