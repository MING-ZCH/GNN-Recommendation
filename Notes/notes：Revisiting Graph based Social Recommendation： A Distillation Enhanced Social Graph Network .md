#  Revisiting Graph based Social Recommendation: A Distillation Enhanced Social Graph Network 

# Basic Information:

- Title: Revisiting Graph based Social Recommendation: A Distillation Enhanced Social Graph Network (重访基于图的社交推荐: 一种蒸馏增强的社交图网络)
- Authors: Ye Tao, Ying Li, Su Zhang, Zhirong Hou, Zhonghai Wu
- Affiliation: School of Software and Microelectronics, Peking University (北大软微), Key Lab of High Confidence Software Technologies (MOE) & National Engineering Center of Software Engineering, Peking University (高可信软件技术教育部重点实验室), Center for Data Science, Peking University (北大数据科学中心), ICBC Technology Co.,Ltd (工商银行科技有限公司)
- Keywords: recommender systems, graph neural networks, social network
- URLs: Paper: https://doi.org/10.1145/3485447.3512003 , GitHub code: https://github.com/xtobelieve/DESIGN

Note: The GitHub link is provided by the authors in the paper.

# 摘要:

- a. 本文的研究背景:
  - 基于社交网络的推荐系统与GNN的应用。
- b. 过去的方法、问题和动机:
  - GNN的应用包含技术成分但缺乏深度思考。
- c. 本文提出的研究方法:
  - DESIGN，即基于知识蒸馏技术训练的增强社交图神经网络。
- d. 本文方法所实现的任务和性能:
  - 取得了超越现有推荐网络的性能。

# 背景:

- a. 主题和特点:
  - 社交网络的推荐系统，包含GNN的应用。
- b. 历史发展:
  - 社交网络的推荐系统分为基于用户和基于物品的推荐两类，GNN的应用是近年来的研究热点。
- c. 过去的方法:
  - 包括基于随机游走的算法和矩阵分解技术。
- d. 过去研究的缺陷:
  - GNN的应用对其自身假设缺乏深度思考。
- e. 需要解决的当前问题:
  - 在推荐系统中更精准地利用社交关系的作用。

# 方法:

- a. 研究的理论基础:
  - 社交网络理论，基于知识蒸馏技术训练的增强社交图神经网络。
  
- b. 文章的技术路线(逐步):
  - 开展社交推荐数据集的统计分析，验证了社交关系对推荐任务的重要性。
  
  - 设计引导GNN社交推荐的度量指标，并证明引入质量较低的社交连接会损害预测性能。
  
  - 提出DESIGN模型，整合用户-物品交互图和用户-用户社交图知识， 并开发两个只使用其中一个图的辅助模型，同时使用知识蒸馏技术进行训练。
  
  - <img src="C:\Users\张辰皓\AppData\Roaming\Typora\typora-user-images\image-20230521231830753.png" alt="image-20230521231830753" style="zoom:23%;" />
  
    <img src="C:\Users\张辰皓\AppData\Roaming\Typora\typora-user-images\image-20230521232030054.png" alt="image-20230521232030054" style="zoom:33%;" />
  
  - 进行实验，通过在现实世界数据集上比较现有技术和DESIGN模型的表现来证明其性能。

# 结论:

- a. 工作的重要性:
  - GNN在推荐领域可持续发展，DESIGN在社交推荐任务中取得了超越现有技术的性能。
- b. 创新、性能和工作负载:
  - DESIGN融合知识蒸馏和社交网络，具有较好的推荐效果，但需要更高的计算工作量。
- c. 研究结论(列出要点):
  - 社交关系与推荐任务的成功相关。
  - 基于用户或基于物品的GNN模型在社交推荐任务中均取得了不错的效果。
  - 社交关系对于构建鲁棒性强的RS模型至关重要。

这篇文章重新审视了现有的基于图神经网络（GNN）的社交推荐方法所做的假设，并提出了Distillation Enhanced Social Graph Network(DESIGN)来提高预测性能。文章通过对广泛使用的社交推荐数据集进行统计分析，验证了社交连接对应推荐任务的重要性，并提出指标来指导GNN社交推荐的使用。作者还尝试将知识蒸馏(KD)技术应用到推荐系统中，提出DESIGN模型，同时使用用户-物品交互图和用户-用户社交图知识进行训练。实验表明，在现实世界数据集上，DESIGN明显优于现有技术。该领域GNN使用于推荐系统，大多数方法依赖用户-物品交互图。在社交推荐方面，引入GNN模型来模拟用户之间的交互过程。文章还讨论了社交推荐方法的一些新方法，并探究了矩阵分解技术在推荐系统中的应用。 作者还提到许多未来研究的方向，包括探索自适应图卷积网络、联合物品推荐和属性推断以及理解图神经网络评估的缺陷。