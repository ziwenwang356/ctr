一，简介

1.FM（factorization machine）模型是一种基于矩阵分解的机器学习模型，对于稀疏数据具有很好的学习能力；

2.FM模型与LR模型的区别在于引进了特征组合；


二，算法

1.线性回归模型：没有考虑特征分量之间的关系；

![Alt text](/Users/wengangwang/Downloads/ctr/fm/linearModel.png "Optional title")

2.考虑特征分量之间关系的线性回归模型：若样本特征为高度稀疏，那么不能对wij参数进行估计，绝大部分为0；

![Alt text](/Users/wengangwang/Downloads/ctr/fm/linearModel2.png "Optional title")

3.FM模型：引入辅助向量vi来对wij进行估计，解决特征稀疏的缺陷；

![Alt text](/Users/wengangwang/Downloads/ctr/fm/fm1.png "Optional title")

![Alt text](/Users/wengangwang/Downloads/ctr/fm/fm1_1.png "Optional title")

![Alt text](/Users/wengangwang/Downloads/ctr/fm/fm1_2.png "Optional title")

4.在实际应用中，一般k值取得比较小，可以限制FM的表达能力，提高模型的泛化能力；


