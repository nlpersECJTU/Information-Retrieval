Paper List for NER

## Nested named entity recognition

- ju等。 A Neural Layered Model for Nested Named Entity Recognition（2018NAACL）[paper](https://www.aclweb.org/anthology/N18-1131/) [code](https://github.com/meizhiju/layered-bilstm-crf)
<br>简介：多数命名实体识别(NER)系统只处理普通实体，而忽略内部嵌套实体，无法捕获底层文本中的细粒度语义信息。为了解决这一问题，我们提出了一种新的神经模型，通过动态叠加平面NER层来识别嵌套实体。

- Wang等。 A Neural Transition-based Model for Nested Mention Recognition（2018EMNLP）[paper](https://www.aclweb.org/anthology/D18-1124/) [code](https://github.com/fishjh2/merge_label)
<br>简介：首先将带有嵌套实体的句子映射到指定的森林，其中每个实体对应于森林的一个组成部分。基于shift-reduce的系统通过一个最大长度保证为句子长度三倍的动作序列，学习以自底向上的方式构建森林结构，在Stack-LSTM的基础上，系统进一步结合了一个基于字符的组件来捕获字母级别的模式。

- Katiyar和Cardie。 Nested Named Entity Recognition Revisited（2018NAACL）[paper](https://www.aclweb.org/anthology/N18-1079/)
<br>简介：提出了一种基于RNN网络的嵌套命名实体识别和嵌套实体提及检测方法，在LSTM网络中加入Top Hidden Layer和label embeddings，提取特征学习嵌套实体的超图表示。

- Zheng等。A Boundary-aware Neural Model for Nested Named Entity Recognition(2019EMNLP)[paper](https://www.aclweb.org/anthology/D19-1034/) [code](https://github.com/thecharm/boundary-aware-nested-ner)
<br>简介：提出了一种基于边界感知的神经网络模型。该模型利用实体边界预测实体类别标签，引入多任务学习方法，捕获实体边界及其分类标签的依赖关系，提高识别实体的性能。

- Fisher和Vlachos。 Merge and Label: A novel neural network architecture for nested NER（2019ACL）[paper](https://www.aclweb.org/anthology/P19-1585.pdf)  [code](https://github.com/fishjh2/merge_label)
<br>简介：引入一种新的神经网络体系结构，它首先将token或实体合并到形成嵌套结构的实体中，然后分别对它们进行标记。与以前的工作不同，我们的合并和标签方法预测实值而不是离散的分割结构，这允许它结合单词和嵌套实体嵌入，同时保持可微性。

- Tan等。 Boundary Enhanced Neural Span Classification for Nested Named Entity Recognition（2020AAAI）[paper](http://www.researchgate.net/publication/342542944_Boundary_Enhanced_Neural_Span_Classification_for_Nested_Named_Entity_Recognition)
<br>简介：提出了一种边界增强型神经跨度分类模型。除了对跨度进行分类之外，还加入一个额外的边界检测任务来预测那些作为实体边界的单词。边界检测模型能够生成高质量的候选跨度，大大降低了推理过程的时间复杂度。

- Wang等。 HIT: Nested Named Entity Recognition via Head-Tail Pair and Token Interaction（2020EMNLP）[paper](https://www.researchgate.net/publication/347234290_HIT_Nested_Named_Entity_Recognition_via_Head-Tail_Pair_and_Token_Interaction)
<br>简介：提出了一种新的嵌套NER模型HIT。提出属于嵌套命名实体的两个关键属性，包括(1)显式的边界字符;(2)边界内字符之间的内部联系紧密。具体地，设计(1基于多头自注意机制的头尾部检测器和双仿射分类器检测边界标记，以及(2)标记交互标记器基于传统的序列标记方法来表征边界内的内部标记连接。

- Luo和Zhao。Bipartite Flat-Graph Network for Nested Named Entity Recognition (2020ACL)[paper](https://www.aclweb.org/anthology/2020.acl-main.571/)  [code](https://github.com/cslydia/BiFlaG)
<br>简介：提出了一种用于嵌套命名实体识别(nested NER)的二部平面图网络(BiFlaG)，该网络包含两个子图模块:一个用于最外层实体的平面平面图模块和一个用于所有位于内层实体的图模块。以前的模型只考虑从最内层到外层(或从外到内)的信息单向传递，而我们的模型有效地捕获了它们之间的双向交互。从图形模块中学习到的更丰富的表示包含了内部实体的依赖关系，可以用来改进最外层实体的预测。

- Wang等。 Pyramid: A Layered Model for Nested Named Entity Recognition（2020ACL）[paper](https://www.aclweb.org/anthology/2020.acl-main.525/) [code](https://github.com/Nicozwy/Pyramid)
<br>简介：提出了一种新的嵌套命名实体识别分层模型——金字塔模型。在本文的方法中，标记或文本区域嵌入递归地输入到平面NER层中，从下到上，以金字塔的形状堆叠。还设计了一个反向金字塔，以允许层之间的双向交互。

- Li等。A Unified MRC Framework for Named Entity Recognition（2020ACL）[paper](https://www.aclweb.org/anthology/2020.acl-main.519/)  [code](https://github.com/ShannonAI/mrc-for-flat-nested-ner)
<br>简介：第一次提出了将嵌套命名实体识别任务转换成机器阅读任务，采用构建数据集中所用的注释指导原则方式生成阅读理解问题，然后利用机器阅读模型求解问题。

- Long等。Hierarchical Region Learning for Nested Named Entity Recognition（2020EMNLP）[paper](https://www.aclweb.org/anthology/2020.findings-emnlp.430/)
<br>简介：为了解决嵌套命名实体文本片段分类方法中存在的问题，运用短语结构中的知识，定义两个相连文本片段的相关程度，根据这个相关程度从底向上生成整个句子的所有候选文本片段，大大降低了时间复杂度，提高嵌套实体识别的性能。

- Xu等。A Supervised Multi-Head Self-Attention Network for Nested Named Entity Recognition（2021AAAI）[paper](https://www.aaai.org/AAAI21Papers/AAAI-6288.XuY.pdf)
<br>简介：以往的方法忽略了词和不同实体类型的语义关联，考虑到词在不同实体中扮演不同的角色，本方法采用监督的多头注意力机制建模头尾词对和每一种实体类型之间的关联，将一个多分类问题转换成N个二分类问题。

- Wang等。Discontinuous Named Entity Recognition as Maximal Clique Discovery（2021ACL）[paper](https://arxiv.org/abs/2106.00218)
<br>简介：将非连续命名实体识别问题转化为寻找句子片段图中最大团的方法。通过网格标记方案，可以在一个阶段内分别生成节点和边，使用新的Mac架构共同学习。

- Li等。A Span-Based Model for Joint Overlapped and Discontinuous Named Entity Recognition（2021ACL）[paper](https://www.researchgate.net/publication/353065282_A_Span-Based_Model_for_Joint_Overlapped_and_Discontinuous_Named_Entity_Recognition) [code]( https://github.com/foxlf823/sodner)
<br>简介：提出了一种新的基于跨的模型，可以同时识别重叠和不连续的实体，首先，通过遍历所有可能的文本范围来识别实体片段，从而识别重叠的实体。其次，我们进行关系分类，以判断给定的一对实体片段是重叠的还是连续的，这样，我们不仅可以识别不连续的实体，同时也可以对重叠的实体进行双重检查。

-Yan等。A Unified Generative Framework for Various NER Subtasks（2021ACL）[paper](https://arxiv.org/abs/2106.01223)  [code]( https://github.com/yhcc/BARTNER)
<br>简介：我们提出将NER子任务定义为一个实体跨序列生成任务，该任务可以通过统一的Seq2Seq框架（BART）解决，利用三种类型的实体表示将实体线性化成一个序列。

## Named entity recognition
- jie等。 Dependency-Guided LSTM-CRF for Named Entity Recognition（2019EMNLP）[paper](https://www.aclweb.org/anthology/D19-1399.pdf)  [code](http://www.statnlp.org/research/information-extraction)
<br>简介：提出了一种简单但高效的依赖指导LSTM-CRF模型，能够编码完整的依赖树，并为命名实体识别任务捕获词的长距离和句法关系——通过这些关系能有效地推断出某些实体。分析表明，显著的改进主要来自依赖树提供的依赖关系和远程交互。

- Ma 等。 Simplify the Usage of Lexicon in Chinese NER（2020ACL）[paper](https://www.researchgate.net/publication/335233357_Simplify_the_Usage_of_Lexicon_in_Chinese_NER)  [code](https://github.com/v-mipeng/LexiconAugmentedNER)
<br>简介：提出了一种简单但有效的方法，将词的信息融合到基于字的表示中，避免了设计复杂的序列标注结构，适用于其他的NER神经网络模型。这种方法基于softword，通过构建BMES集合的方式获取词的信息，最后将词的信息融合到字的表示中。

- Xu等。Better Feature Integration for Named Entity Recognition（2021NAACL）[paper](https://arxiv.org/abs/2104.05316)
<br>简介：我们都知道从依存句法树中获取的长距离结构信息对命名实体识别性能提高有帮助，通常的做法是堆叠使用LSTM和图神经网络建模上下文信息和结构信息，然后这两者信息的交互形式不明确，而且性能提高不是很明显，所以本文通过更改LSTM中门控机制的方法将结构信息融入LSTM中，因此能明确两部分信息的交互。

- Lin等。TriggerNER: Learning with Entity Triggers as Explanations for Named Entity Recognition（2020ACL）[paper](https://www.aclweb.org/anthology/2020.acl-main.752/) [code](http://github.com/INK-USC/TriggerNER)
<br>简介：对于一个新的领域，要构建命名实体识别神经网络模型就需要大量的标注数据，这往往是昂贵且耗时的，本文提出对语料进行“实体触发器”的标注，提出触发器匹配网络模型TMN，联合学习触发器表示和具有自注意的软匹配模块，从而可以很容易地泛化到对无监督句子进行标注，通过这种额外的标注可以促进实体识别模型标签的高效学习。

## Others
- Tian等。 - Joint ChineseWord Segmentation and Part-of-speech Tagging via Two-way Attentions of Auto-analyzed Knowledge（2020ACL）[paper](https://www.aclweb.org/anthology/2020.acl-main.735/)
<br>简介：提出了一种用于中文分词和词性标注联合任务的神经网络模型TWASP，遵循基于字符的序列标注，使用双向注意机制将每个输入字符的上下文特征及其对应的句法知识结合起来。双向注意机制用于结合上下文特征及其对应的语法知识的每个输入字符，使用现有的语言处理工具包来获取上下文的自动分析语法知识。
