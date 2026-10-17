# THINKING.md · 开工前必读

> 每次回答前查看本文件。它是本工作区的常驻工作约定，不是文档。

## 当前任务上下文

- 本工作区（Lemma AI Analysis Engine）是 Analysis Engine 研究的原型/草稿空间。
- **正式研究仓库：`D:\github projects\analysis-engine-research`**（2026-10-17 初始化，
  本地 git，无远端）。结论性东西落那个仓库，不落这里。

## 工作原则（从任务约定与既往反馈固化）

1. **结论先行，每条一句，10–20 字，不解释为什么。** AI 味来自解释从句和自我点评，
   不来自词汇。宁可少写，不要写满。
2. **观察 / 推断 / 假设 / 决策四分**，不混为一句无限定断言。写结论时先归层。
3. **不编造无定义的数字**：没有置信度、没有百分比、没有评分，除非定义了含义。
4. **不重新引入四层元认知模型（L1–L4）或任何等价固定层级** —— lemma-ai 已正式撤回。
5. **合成数据只检验计算行为**，禁止外推"建模了人类认知"。
6. **每个实验先写可证伪假设与反对条件，再写代码**；负面结果与正面结果同权。
7. **lemma-ai 只读参考**：不切分支、不改文件；读分支内容用
   `git show/ls-tree/grep <branch>:<path>`（沙箱会挡 `.git/index.lock`，
   `git status` 之类会触发授权）。
8. 交付前回读自查：术语残留、行号引用、过期文件点名。

## 环境备忘

- 本机托管 Python：`C:/Users/chkev/.workbuddy/binaries/python/envs/default/Scripts/python.exe`
  （numpy 2.5.4 / pytest 9.1.1）。
- Bash 写 `D:\github projects\analysis-engine-research` 会被沙箱拦截；
  文件改动用写工具，跑命令时加 `PYTHONDONTWRITEBYTECODE=1` 避开 `__pycache__` 噪音。
- Windows 程序不认 `/c/` 路径，用 `C:/...`。
