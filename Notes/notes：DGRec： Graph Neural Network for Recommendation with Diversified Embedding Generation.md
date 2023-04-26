# DGRec: Graph Neural Network for Recommendation with Diversified Embedding Generation 

# Basic Information:

- Title: DGRec: Graph Neural Network for Recommendation with Diversified Embedding Generation (图神经网络推荐算法的多元嵌入生成方法)
- Authors: Liangwei Yang, Shengjie Wang, Yunzhe Tao, Jiankai Sun, Xiaolong Liu, Philip S. Yu, and Taiqing Wang
- Affiliation: University of Illinois at Chicago (芝加哥伊利诺伊大学)
- Keywords: Graph Neural Network, Recommendation System, Submodular Function
- Urls: https://doi.org/10.1145/3539597.3570472, Github:https://github.com/YangLiangwei/DGRec

# Summary:

- a. Research background of this article:
  - 本文旨在通过子模函数和图神经网络(DGRec)结合，提出一种高效多样的推荐系统，以提高推荐多样性和用户体验。
- b. Past methods, their problems, and motivation:
  - 以往的推荐系统依赖于高度相关的项，会导致推荐雷同性增加，情况尤其严重在多样性推荐任务中。
- c. Research methodology proposed in this paper:
  - DGRec利用面向图的神经网络的推荐系统生成用户和项的嵌入，通过三个主要模块实现有效的推荐多样性：子模邻居选择、层关注和损失重加权。
- d. Task and performance achieved by the methods in this paper:
  - DGRec旨在提高推荐系统多样性，有效管理大规模推荐任务，通过子模函数和高效算法，达到良好的优化和增强推荐多样性的效果。

# Background:

- a. Subject and characteristics:
  - 本文研究的主题是推荐系统多样性，即在保持推荐准确性的前提下，提高推荐项的多样性。
- b. Historical development:
  - 以往的推荐方法依赖于高度相关的项，会导致推荐雷同性增加。
- c. Past methods:
  - 过去的推荐系统通常使用相关性来推荐高度相似的项。
- d. Past research shortcomings:
  - 另一方面，这种方法缺乏推荐多样性，可能会导致对长尾项的低覆盖和推荐饱和问题。
- e. Current issues to address:
  - 因此，当前需要解决的问题是提高推荐系统的多样性，同时保持准确性和可伸缩性。

# Methods:

- a. Theoretical basis of the study:

  - DGRec是一个多样化推荐系统，结合了子模函数和图神经网络的推荐系统生成用户和项的嵌入。

- b. Technical route of the article (step by step):

  - DGRec有三个主要模块：
    - 子模邻居选择模块：从图结构中选择一组多样化邻居，并使用设施位置函数评估所选子集的多样性。
    - 层关注模块：计算每个层输出对最终表示的重要性，并将每个层的输出乘以其重要性权重。
    - 损失重加权模块：通过加权损失函数来强调长尾类别。

- c. Algorithms and models:

  - DGRec使用了子模函数来评估多样性，图神经网络用于生成用户和项的嵌入，利用AGG和子模选择模块来减少邻近节点信息的影响。

- d. Data collection and analysis:

  - 本研究使用用户-项目二分图作为训练数据，使用具有代表性的数据集进行评估（MovieLens 和 Yelp)。

  # Conclusion:

- a. Significance of the work:

  - DGRec是一种有效解决推荐系统多样性的方法，能够提供优化和增强推荐多样性的效果。

- b. Innovation, performance, and workload:

  - DGRec通过使用子模选择和高效算法来减少邻近节点信息的影响，同时通过层关注和损失重加权的计算来增强数据集中的推荐多样性，提高了算法的性能。

- c. Research conclusions:

  - 本文提出的DGRec方法具有很好的准确性、拓展性和数据稳定性，在多个推荐任务数据集上都获得了很好的结果。