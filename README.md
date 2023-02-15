# ChatGPT 涉及开源软件研究
ChatGPT涉及到的开源软件如下：
1. https://github.com/LAION-AI/Open-Assistant
1. https://github.com/CarperAI/trlx
1. https://github.com/lucidrains/PaLM-rlhf-pytorch

LAION，即 Large-scale Artificial Intelligence Open Network，是一个非盈利的机器学习研究机构，致力于为公众提供 AI 模型、数据集和代码。2022 年， LAION 发布的LAION-5B，这是一个包含超过 50 亿个图像文本对的人工智能训练数据集。LAION 的最新项目是 OpenAssistant，旨在“让每个人都可以访问基于聊天的大型语言模型”。计划中的 OpenAssistant MVP 实现将基于 OpenAI 的 InstructGPT 论文：人工生成指令的数据集、机器生成的响应及其人类排名的数据集，以及 RLHF 的实现。根据 LAION 的说法：

"我们不会止步于复制 ChatGPT。我们希望构建未来的助手，不仅能够编写电子邮件和求职信，还能做有意义的工作、使用 API、动态研究信息等等，并且能够由任何人进行个性化和扩展。我们希望以一种开放和可访问的方式来做到这一点，这意味着我们不仅要构建一个出色的助手，还要使其足够小且高效以在消费类硬件上运行。"

CarperAI 是EleutherAI研究小组的一个新实验室，其任务是“通过强化学习提高大型语言模型 (LLM) 的性能和安全性。” InfoQ 之前报道过 EleutherAI 开发的开源语言模型GPT-NeoX。2022 年 10 月，该实验室宣布了一个使用 RLHF训练和公开发布“指令调整”模型的项目。该项目是几个组织的合作成果，包括HuggingFace、Scale和Humanloop。作为该项目的一部分，CarperAI 开源了 Transformer Reinforcement Learning X (trlX)，这是一个使用 RLHF 微调 HuggingFace 语言模型的框架。

以Imagen和Make-A-Video等深度学习研究模型的开源实现而闻名的 AI 开发人员 Phil Wang分享了他正在为PaLM语言模型（称为 PaLM + RLHF）实施 RLHF 的工作。Wang 指出，没有预训练模型，只有用户自己训练的框架。他还建议有兴趣复制 ChatGPT 的用户加入LAION discord 频道。

尽管这些开源项目包括 ChatGPT 训练方法的实现，但它们目前没有任何可用的训练模型。Wang 的项目常见问题解答表明，培训可能需要“数百万美元的计算 + 数据”才能完成。LAION 的OpenAssistant路线图文档确实列出了收集数据和训练模型的工作，但不清楚何时可以发布经过训练的模型。CarperAI 的 Twitter 帐户指出：

"我们还没有正式发布任何 RLHF 模型，只是 hh-RLHF 的一些小复制工作，学习总结等在我们的 discord 中。我们可以匹配各自论文中报告的性能。"

人工智能社区的几位知名成员在社交媒体上讨论了这些努力。在 Twitter 上，HuggingFace 首席技术官 Julien Chaumond预测，在六个月内将有“10 个 ChatGPT 的公开复制品”。AI 研究员 Sebastian Raschka回复道：

"同意，将会有许多 ChatGPT 的开源实现。但是不会有很多高质量的模型。我认为我们低估了人们讨厌手工标记（或更糟：编写）训练数据的程度。"

StabilityAI 的创始人 Emad Mostaque 在推特上表示，他的公司正在“致力于开放聊天 GPT”。他还说：

"创建开放聊天 GPT 最困难的部分（除了 RL 位的数百万美元）是治理方面......好消息是一旦所有的血汗和泪水都投入到创建模型和框架中，它们就可以像新类型一样疯狂地扩散开发原语。"

软件容易解决，训练数据集及训练模型估计需要数百万美元
