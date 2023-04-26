# Disentangled Graph Social Recommendation 

# Basic Information:

- Title: Disentangled Graph Social Recommendation (解析图社交推荐)
- Authors: Lianghao Xia, Yizhen Shao, Chao Huang, Yong Xu, Huance Xu, Jian Pei
- Affiliation: University of Hong Kong (香港大学), South China University of Technology (华南理工大学), Duke University
- Keywords: social recommendation, graph neural network, latent factors
- Urls: https://ieeexplore.ieee.org/document/9267663, Github: https://github.com/HKUDS/DGNN

# Summary:

- (1): 本文研究社交推荐系统中异构关系的表示问题。
- (2): 传统方法缺乏对物品语义相关性的探索，无法在实际场景中提供准确的推荐。研究者提出了一种基于图神经网络的异构存储器增强消息传递的Disentangled Graph Neural Network（DGNN）方法，以在复杂的社交情境中有效提高用户偏好学习。该方法能够自动捕捉异构关系与不同关系之间的混合关系，从而提高了推荐的精度。
- (3): 本文提出的DGNN方法利用异构图存储器增强消息传递，通过分离残差层、设计多跳邻居关系层和不同函数的区分网络阶段，捕捉不同节点和边类型之间的关系异构性和潜在因素的交错。在捕捉混合关系、解决特征不变性和模型可解释性等方面较传统模型具有更好的表现。
- (4): 本文提出的DGNN方法应用于社交推荐领域中的真实数据集上，比多个现有的推荐技术表现更优，特别是在考虑异构关系的情况下。

# Background:

- a. Subject and characteristics:
  - 本文研究社交推荐系统中的异构关系，并提出了相应的解决方案。
- b. Historical development:
  - 社交网络是推荐系统中已被广泛应用的一种关系类型。然而，传统的社交感知推荐方法存在着一些问题，无法很好地处理混合优化和异构关系等问题。
- c. Past methods:
  - 过去的方法主要是基于矩阵分解、深度神经网络等模型进行建模的。但这些方法无法处理异构关系，因此无法在实际场景中提供准确的推荐。
- d. Past research shortcomings:
  - 过去的研究方法无法很好地处理混合优化和异构关系等问题。
- e. Current issues to address:
  - 在真实场景下，异构关系的表示问题是社交推荐系统发展中的一个重要瓶颈。

# Methods:

- a. Study's theoretical basis:
  - 本文主要基于图神经网络的框架，利用异构图存储器增强消息传递，进行对推荐模型的改进。
- b. Article's technical route (step by step):
  - 本文提出的DGNN模型通过多跳邻居关系层和不同函数的区分网络阶段来捕捉不同节点和边类型之间的关系异构性和潜在因素的交错。此外，本文还设计了分离残差层，以捕捉混合关系、解决特征不变性和模型可解释性等问题。

# Conclusion:

- a. Work significance:
  - 本文提出的DGNN方法解决了传统众多推荐技术所存在的无法很好地处理混合优化和异构关系等问题，对推荐系统领域的发展有重要的参考价值。
- b. Innovation, performance, and workload:
  - 本文提出的DGNN模型通过多跳邻居关系层和不同函数的区分网络阶段，解决了传统模型无法处理异构关系的问题，并在真实数据集上表现出卓越的性能。
- c. Research conclusions (list points):
  - 本文提出一种利用graph neural networks（GNN）解决社交推荐系统中的异构关系表达问题的方法；
  - 本文设计并实现了disentangled graph neural networks（DGNN）模型，用于处理社交网络中复杂的异构关系，提高推荐的精度；
  - 本文的方法采用了多跳邻居关系层和不同函数的区分网络阶段，能够自动捕捉异构关系，提高用户偏好学习。