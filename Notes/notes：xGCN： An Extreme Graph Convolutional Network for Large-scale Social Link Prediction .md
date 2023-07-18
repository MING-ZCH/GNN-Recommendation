#  xGCN: An Extreme Graph Convolutional Network for Large-scale Social Link Prediction  

# Basic Information:

- Title: xGCN: An Extreme Graph Convolutional Network for Large-scale Social Link Prediction (xGCN：一种用于大规模社交链接预测的极限图卷积网络)
- Authors: Xiran Song, Jianxun Lian, Hong Huang, Zihan Luo, Wei Zhou, Xue Lin, Mingqi Wu, Chaozhuo Li, Xing Xie, and Hai Jin
- Affiliation: Xiran Song and Hong Huang are affiliated with the National Engineering Research Center for Big Data Technology and System, Services Computing Technology and System Lab, Cluster and Grid Computing Lab, School of Computer Science and Technology, Huazhong University of Science and Technology.
- Keywords: Link prediction, graph neural network, social recommendation
- URLs: Paper: https://doi.org/10.1145/3543507.3583340, GitHub: None

# Summary:

- a. Research background of this article:

  - 用于图结构表示的图神经网络（GNNs）被广泛使用，然而，它们在归纳学习任务中的表现仍然具有挑战性。

- b. Past methods, their problems, and motivation:

  - GNN有大量的可训练参数，并且是基于堆叠邻域聚合，这会降低其效率和可扩展性。

- c. Research methodology proposed in this paper:

  - 本文提出了一种新的GNN，称为xGCN，它使用极端卷积方法对图结构数据进行编码。xGCN没有给每个节点分配一个直接可学习的嵌入向量，而是将节点嵌入视为静态特征，并使用传播操作来平滑节点嵌入。

- d. Task and performance achieved by the methods in this paper:

  - 在三个带有链接预测任务的社交网络数据集上的实验表明，与一系列有竞争力的基础模型相比，xGCN不仅达到了最好的准确性，而且具有很高的效率和可扩展性。

  # Background:

- a. Subject and characteristics:

  - 本文主要讨论图神经网络（GNN）及其在表示图结构数据方面的应用，具体重点是归纳学习任务。

- b. Historical development:

  - GNN已被广泛使用，然而，其准确性、效率和可扩展性仍是挑战。

- c. Past methods:

  - 过去的方法包括GNN，它有大量的可训练参数，并且是基于堆叠邻域聚合的。

- d. Past research shortcomings:

  - 过去的研究表明，这些过去的方法降低了效率和可扩展性，从而限制了其性能。

- e. Current issues to address:

  - 作者指出，GNN的准确性、效率和可扩展性仍然具有挑战性，需要有更有效的方法来解决这些问题。

# Methods:

- a. Theoretical basis of the study:

  - xGCN以极端卷积的方式对图结构数据进行编码，使用传播操作来平滑节点嵌入，并依靠精化神经网络（RefNet）将无监督传播得到的粗略嵌入转化为优化训练目标的新嵌入。

- b. Technical route of the article (step by step):

  - 所提出的模型，xGCN，涉及三个关键操作：嵌入传播，嵌入细化，和嵌入刷新。它将节点嵌入视为静态特征，并使用一个细化神经网络，而不是一个可训练的嵌入表。RefNet通过一个成对的排名损失函数进行训练，以提取有用的信号并过滤掉噪音。训练过程使用一个预热阶段来协调嵌入刷新和细化之间的关系。

- c. Innovation and performance:

  - xGCN效率高，可扩展性强，在社会链接预测任务中取得了优异的成绩，超过了其他基线模型，如GraphSAGE、GAT、GIN、SGC、S2GC、SIGN、GBP、PPRGo和LightGCN。

  # Conclusion:

- a. Significance of the work:

  - 所提出的xGCN方法解决了GNN中的准确性、效率和可扩展性问题，并在社会链接预测任务中取得了优异的成绩。

- b. Innovation, performance, and workload:

  - xGCN采用极端的卷积方法和细化神经网络，改变了传统的GNN范式，实现了高效、可扩展和高度准确的社会链接预测。

- c. Research conclusions (list points):

  - xGCN效率高、可扩展，在社会链接预测任务中与基线模型相比产生了卓越的结果。所提出的模型采用极端卷积方法和细化神经网络，改变了传统的GNN范式，解决了GNN中的准确性、效率和可扩展性问题。嵌入传播、细化和刷新操作确保了该模型在不同的社交网络中是有效和稳健的。