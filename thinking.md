最近我学习到一个很有用的知识： 语言模型的定义是什么？ 给定上文（context），model能输出下一个 token 的概率分布。

这里面包含不可缺少的东西： 1. context 2. 概率分布，即model parameters。这两者同时决定了LLM现在知道什么： context来自外部，model parameters来自模型本身。



最近我开始思考，在Agent时代， Context和 model parameters之间的关系是什么？ 




最早的时候，人们使用小模型+外部知识库来做LLM， 小模型可以retrieve外部直属库来获取knowledge帮助他解决任务，也就是RAG。这些knowledge就是包含了LM对外部世界的理解，即world。


后来，人们发现scaling 模型的参数能够使得模型的能力进一步提升， 模型能够利用参数记住一些知识帮助他们解决外部世界的任务； 人类通过post-training进一步refine这些知识，使其更加符合现在人类社会的认知。这时， parameterized knowledge即是LLM的world。


现在， agent时代，LLM可以通过tools 或者harness设计来获取或者编排外部世界的知识， 让LLM能够及时access最新且真实的世界知识。
