# Graph Attention Networks 

# Basic Information:

- Title: Graph Attention Networks (图形注意力网络)
- Authors: Petar Veličković, Guillem Cucurull, Arantxa Casanova, Adriana Romero, Pietro Liò, Yoshua Bengio
- Affiliation: Department of Computer Science and Technology, University of Cambridge (剑桥大学计算机科学与技术系)
- Keywords: graph attention networks, neural networks, self-attention, graph-structured data, inductive learning
- URLs: [Paper](https://arxiv.org/abs/1710.10903), [GitHub](https://github.com/PetarV-/GAT)

Note: While the first author (Petar Veličković) was at the Montréal Institute of Learning Algorithms when the research was conducted, the affiliation listed on the first page of the paper is their current affiliation at the time of publication (University of Cambridge).

# 摘要：

- a. 本文研究背景：
  - 本文提出了基于图注意力网络(GATs)，通过使用掩码自注意层，解决了之前基于图卷积或其近似方法在处理图结构数据时的局限性。
- b. 过去的方法，问题及动机：
  - 过去的方法中，基于图卷积或其近似方法在处理图结构数据时有局限性，没有很好的考虑节点的邻域特征。作者通过引入掩码自注意层并使节点自注意到其邻域特征来解决这个问题。
- c. 本文提出的研究方法：
  - 在图卷积和其近似方法的基础上，本文提出了一种基于图注意力网络的方法，通过自注意层聚合特征信息并将不同节点赋予不同权重。
- d. 方法在任务中的表现：
  - 本文提出的方法在多个图结构数据集上进行了测试，包括Cora、Citeseer、Pubmed引文网络数据集以及蛋白质相互作用数据集，表现出了与先进水平相当的表现。该方法在处理不同大小的图输入时表现出了高效且可并行的特性。

# 背景：

- a. 主题和特征：
  - 本文探讨了基于图结构数据的机器学习算法，着重研究了如何处理局部相关的信息。
- b. 历史发展：
  - 历史上出现了基于图卷积、近似计算等方法，但它们在处理图结构数据时存在很多局限性，无法充分利用节点的邻域信息。
- c. 过去的方法：
  - 过去的方法中存在一些基于图卷积和其近似方法的算法。
- d. 过去研究的缺陷：
  - 过去的方法往往无法充分利用节点的邻域信息，导致任务表现不尽如人意。
- e. 当前需要解决的问题：
  - 如何在处理图结构数据时充分利用节点邻域的信息，同时保证算法的高效性和可扩展性。

# 方法：

- a. 研究的理论基础:

  - 本文的研究基于图注意力网络的思想，通过自注意层实现了节点邻域信息的聚合。

- b. 文章的技术路线(逐步):

  - 本文的方法主要包括一个基于图的自注意层，该层通过对节点的邻域特征进行自注意，实现了特征的聚合以及节点权重的分配。该层可以通过堆叠形成深层网络结构。由于注意力机制是在整个图中共享的，因此该方法具有很好的可扩展性，能够处理不同大小的图。同时，该方法的权重变化是由节点自注意的得到的，因此可以处理未见过的测试图像。该方法也可以很容易地扩展到多头自注意机制，并可以通过跳过连接技术等方法进一步增加深度。

    #  结论：

- a. 本文的研究意义：

  - 本文提出了一种新的图注意力网络方法，可以更好地处理图结构数据，具有很好的可扩展性和高效性。

- b. 创新、性能和工作量：

  - 本文提出的方法不仅在多个图结构数据集上表现出与当前最先进技术相当的性能，而且具有很好的可扩展性和高效性，可解决以前方法的一些缺陷。

- c. 研究结论 (列出要点):

  - 本文提出的图注意力网络(GATs)可以有效地处理未见过的测试图像，并在多个数据集上取得了良好的性能。