# NER-papers
Paper List for NER
- Tan等。Boundary Enhanced Neural Span Classification for Nested Named Entity Recognition（AAAI2020） 提出了一种边界增强型神经跨度分类模型。除了对跨度进行分类之外，还加入一个额外的边界检测任务来预测那些作为实体边界的单词。边界检测模型能够生成高质量的候选跨度，大大降低了推理过程的时间复杂度。[paper](http://www.researchgate.net/publication/342542944_Boundary_Enhanced_Neural_Span_Classification_for_Nested_Named_Entity_Recognition)
- Zheng 等。 - 2019 - A Boundary-aware Neural Model for Nested Named Entity Recognition(EMNLP2019)  提出了一种基于边界感知的神经网络模型。该模型利用实体边界预测实体类别标签，引入多任务学习方法，捕获实体边界及其分类标签的依赖关系，提高识别实体的性能。[paper](https://www.aclweb.org/anthology/D19-1034/) [code](https://github.com/thecharm/boundary-aware-nested-ner)
- Tian 等。 - Joint ChineseWord Segmentation and Part-of-speech Tagging via Two-way Attentions of Auto-analyzed Knowledge（ACL2020）。提出了一种用于中文分词和词性标注联合任务的神经网络模型TWASP，遵循基于字符的序列标注，使用双向注意机制将每个输入字符的上下文特征及其对应的句法知识结合起来。双向注意机制用于结合上下文特征及其对应的语法知识的每个输入字符，使用现有的语言处理工具包来获取上下文的自动分析语法知识。[paper](https://www.aclweb.org/anthology/2020.acl-main.735/)
