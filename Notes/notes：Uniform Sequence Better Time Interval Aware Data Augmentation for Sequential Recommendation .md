#Uniform Sequence Better: Time Interval Aware Data Augmentation for Sequential Recommendation  

# Basic Information:

- Title: Uniform Sequence Better: Time Interval Aware Data Augmentation for Sequential Recommendation (均匀序列优化：考虑时间间隔的序列推荐数据增强)
- Authors: Yizhou Dang, Enneng Yang, Guibing Guo, Linying Jiang, Xingwei Wang, Xiaoxiao Xu, Qinghui Sun, Hong Liu
- Affiliation: Software College, Northeastern University, China
- Keywords: Sequential recommendation, Time interval, Data augmentation, Uniform sequence, Non-uniform sequence
- URLs: arXiv:2212.08262v1 [cs.IR] 16 Dec 2022, GitHub: https://github.com/KingGugu/TiCoSeRec

# 方法:

- a. 理论背景:
  - 本文提出了一种针对顺序推荐的时间间隔感知数据增强方法，该方法考虑了序列中交互项之间的时间间隔分布。现有的顺序推荐方法主要关注基于物品排序序列建模用户偏好，但忽视了时间间隔因素，可能导致偏好漂移。作者进行了实证研究，表明具有均匀分布时间间隔的序列比具有差异较大时间间隔的序列对性能改进更有益。为了解决非均匀序列的问题，作者提出了五种数据增强操作（Ti-Crop、Ti-Reorder、Ti-Mask、Ti-Substitute、Ti-Insert），并采用控制策略处理短序列的数据增强。作者在一种先进模型上实现了这些改进，并在四个真实数据集上验证了他们的方法。实验结果表明，与其他11个竞争模型相比，他们的TiCoSeRec方法取得了显著的性能改进。这项工作通过考虑给定序列的时间间隔分布填补了顺序推荐模型的研究空白。数据增强已被广泛用于提高推荐性能，本文提出了一种考虑时间间隔因素的新方法。
- b. 技术路线:
  - 本文提出了一种顺序推荐中的数据增强方法，该方法考虑了动作之间的时间间隔。作者验证了均匀序列对于下一个物品预测更有价值的假设，并提出了五种基于时间间隔的数据操作符来增强物品序列。作者在四个公共数据集上评估了所提出方法的有效性，并且其性能明显优于现有方法。作者还进行了消融研究，展示了所提出的数据操作符的有效性以及参数sigma对推荐准确性的重要性。未来，作者计划将物品类别作为数据增强的因素进行考虑。

# 结果:

- a. 详细的实验设置:
  - 作者在四个公共数据集上进行了实验评估，具体数据集名称未提及。
  - 作者使用了一种先进模型进行实现，并对该模型进行了改进。
  - 作者使用了五种数据增强操作（Ti-Crop、Ti-Reorder、Ti-Mask、Ti-Substitute、Ti-Insert）来处理物品序列。
  - 作者采用了控制策略来处理短序列的数据增强。
- b. 详细的实验结果:
  - 作者的TiCoSeRec方法在四个真实数据集上取得了显著的性能改进。
  - 作者进行了消融研究，证明了所提出的数据操作符的有效性。
  - 作者强调了参数sigma对推荐准确性的重要性。
  - 作者计划将物品类别作为数据增强的因素进行考虑。