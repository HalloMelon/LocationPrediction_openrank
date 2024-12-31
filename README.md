# LocationPrediction_openrank
开发者地理位置信息在开源数据分析中对于理解全球开源活动的分布及制定区域政策至关重要，从而引起了学术界的广泛关注。然而，大多数现有研究主要依赖开发者在GitHub上填写的地理位置信息，而如何从用户的其他信息中挖掘其地理位置是一项具有挑战性的任务。为此，本文提出了一种基于BiLSTM的GitHub开发者地理位置预测框架。该框架首先综合考虑了用户的个人简介、邮箱域、公司信息、姓名及活跃度等多维数据，并通过应用Moonshot大模型，有效扩展了开发者地理位置信息。然后，通过基于BiLSTM的地理位置预测方法，结合开发者活跃时间序列以及开发者个人画像的多个特征来推测其地理位置。实验结果表明，通过捕获开发者协作行为日志数据的时序特征，BiLSTM相比其他基线方法在预测精度上表现优异，准确率达到0.684。进一步分析主要开源参与国的用户分布与活跃时间特征，本文揭示了全球开源活动的空间分布模式和时间特性，为深入研究各国开源贡献提供了一定参考。

- 整体的思路框架如下图所示：

<img src="pics\method.jpg" width="700">

- 如下图所示，美国拥有最多的活跃用户，表明其在全球开源生态系统中的绝对领导地位。其次，印度、德国、英国、中国和巴西的开发者数量位居前列，代表了全球开源社区中具有显著增长潜力的区域市场。这些国家的用户数量和参与度突显了北美和西欧在开源生态中的核心地位，同时也反映了新兴经济体（如印度和中国）在开源领域日益扩展的参与度和影响力。这种地理分布模式反映了不同国家在技术发展阶段、开源文化接受度以及科技基础设施建设上的差异。美国和欧洲在开源社区中的领先地位，主要归因于其长久以来在信息技术研发、教育资源等方面的优势。美国的开源开发者数量远超其他国家，反映了其在创新和开源文化推广上的高度成熟度与生态化体系。

<img src="pics\map.png" width="700">