# Yueqi Chen

我是厦门大学计算机专业的本科生，关注计算机领域前沿发展并尝试进行计算机视觉领域相关研究。我把学习中遇到的问题做成浏览器里的交互实验，也为整理课堂资料、检查数据和发布项目写工具。

I'm a computer science undergraduate at Xiamen University. I follow advances in computing and am exploring research questions in computer vision. I build interactive experiments in stereo geometry and machine learning, and contribute bug fixes to open-source Python projects.

[个人网站](https://chenyueqi2024.github.io/) · [成长手记与开源经历](https://chenyueqi2024.github.io/academic/) · [个人小天地](https://chenyueqi2024.github.io/life/)

## 视觉与机器学习 · Vision & ML

- **视角游乐场 · Viewpoint Playground**　为什么远处物体的深度更难测准？拖动双目相机和目标，观察左右画面中的视差，再打开测量噪声，比较多次估计得到的深度分布。[动手测深度](https://chenyueqi2024.github.io/viewpoint-playground/) · [源码](https://github.com/ChenYueqi2024/viewpoint-playground)
- **Model Mechanics**　19 个中文交互实验，从语言 token 讲到图像、训练和决策。语言 Transformer 和 ViT 共用同一段计算代码，可以先关闭前馈层，再到视觉课移除一个图块，比较两种改动对输出的影响。[课程目录](https://chenyueqi2024.github.io/model-mechanics/) · [语言 Transformer](https://chenyueqi2024.github.io/model-mechanics/transformer/) · [ViT 实验](https://chenyueqi2024.github.io/model-mechanics/vit/)
- **多视角数据体检 · Multiview Check**　在开始重建前，先核对图片尺寸、相机内参、位姿和时间戳。可以先看一份故意放入异常的合成数据报告，再用浏览器或 Python 在本机检查自己的数据。[查看异常报告](https://chenyueqi2024.github.io/multiview-check/demo-report.html) · [检查自己的数据](https://chenyueqi2024.github.io/multiview-check/) · [源码](https://github.com/ChenYueqi2024/multiview-check)

## 人工智能安全 · AI Safety & Security

我关注大模型系统的安全与可靠性，尤其是检索增强生成（RAG）和工具型智能体如何处理不可信输入、保护私有资料，以及限制真实操作。我用可复现的交互实验研究安全控制在哪一步起作用，以及它会不会挡住正常任务。

I’m interested in AI safety and security, particularly how retrieval-augmented systems and tool-using agents handle untrusted inputs, protect private data, and enforce action permissions. I build interactive experiments to study where safeguards help and when they block legitimate tasks.

- **大模型权限与安全评估 · LLM Safeguards & Evaluation**　用规则沙盒观察不可信资料如何影响候选操作，再用同一批合成案例对照多套权限策略，分别衡量上下文曝光、越权放行和误拒。[权限沙盒](https://chenyueqi2024.github.io/explore/ai-security/) · [AI 安全评估](https://chenyueqi2024.github.io/explore/ai-safety-eval/)
- **证据与模型可靠性 · Evidence & Reliability**　检查 RAG 的回答是否有足够证据，比较置信度和实际正确率，观察何时该拒答或转人工复核。[RAG 证据实验](https://chenyueqi2024.github.io/model-evidence-labs/rag/) · [置信度与校准](https://chenyueqi2024.github.io/model-evidence-labs/calibration/)
- **网络与信息安全 · Networking & Information Security**　通过网页请求、TLS、密码学和密文计算的实验，理解大模型应用沿用的系统信任边界。[专题目录](https://chenyueqi2024.github.io/explore/#security)

## 学习与开发工具 · Tools

- **公开之前 · before-public**　公开文件前，用浏览器在本机检查照片里的 GPS 信息，也能用中英文 OCR 查找图片和扫描 PDF 中的敏感文字。命令行版还可以检查 Git 暂存区和提交历史。[试用合成样例](https://chenyueqi2024.github.io/before-public/) · [源码与命令行用法](https://github.com/ChenYueqi2024/before-public)

- **SlidePatch** — 把已有 PowerPoint 内容迁移到新模板，保留可编辑的文字和原生图表。项目页有封面、正文和图表的迁移前后对比。[查看对比](https://github.com/ChenYueqi2024/SlidePatch#readme) · [下载](https://github.com/ChenYueqi2024/SlidePatch/releases)
- **问迹 · Wenji** — Android 课堂疑问与复习助手。随手记下问题，导入讲义后核对引用，再用复习卡练习独立作答。[项目说明](https://github.com/ChenYueqi2024/wenji#readme) · [APK 下载](https://github.com/ChenYueqi2024/wenji/releases)
- **dsh-memory** — 为 DeepSeek Harness 保存工作区的约定、决策和偏好，让新会话接上同一项目的上下文。[网站与演示](https://chenyueqi2024.github.io/dsh-memory/) · [项目源码](https://github.com/ChenYueqi2024/dsh-memory)

## 开源贡献 · Selected pull requests

- **eslint-plugin-jsdoc · 已合并**　修复自动转换 `/// Section` 等注释时意外生成 `*/`、导致 JavaScript 无法解析的问题，并补充 8 个回归用例。[PR #1848](https://github.com/gajus/eslint-plugin-jsdoc/pull/1848)
- **fsspec** — 为 HTTP 目录探测限制读取量，避免为了判断目录而下载大文件。[PR #2465](https://github.com/fsspec/filesystem_spec/pull/2465)
- **PEtab** — 按测量条件对齐模拟结果，避免乱序数据让散点和回归统计失真。[PR #612](https://github.com/PEtab-dev/libpetab-python/pull/612)
- **pyinfra** — 让 SSH 配置的一条 `Include` 指令能读取多个路径，并补充读取顺序的回归测试。[PR #2090](https://github.com/pyinfra-dev/pyinfra/pull/2090)
