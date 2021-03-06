### Metric

> 网络结果的度量标准


### 1.
 * 一些定义：
   * TP : 正样本，预测正确，预测为正样本，真正样本
   * FN : 正样本，预测错误，预测为负样本，假负样本
   * FP : 负样本，预测错误，预测为正样本，假正样本
   * TN : 负样本，预测正确，预测为负样本，真负样本
   * P : 所有正样本，即 TP + FN
   * N : 所有负样本，即 FP + TN
 
 * 一些概念：
   * FPR = FP/N
      * False Positive Rate，假正率：所有“负样本”（FP+TN）中，预测为正样本的占比
   * TPR = TP/P
      * True Positive Rate，真正率：所有“正样本”（TP+FN）中，预测为正样本的占比
   * precision = TP/(TP+FP) 
      * 精确率：所有“预测为正样本的样本”（TP+FP）中，本来是正样本的占比
   * recall = TP/P
      * 回收率：所有“正样本”（TP+FN）中，预测为正样本的占比
   * accuracy = (TP+TN)/(P+N)
      * 正确率：所有样本中，预测正确的样本的占比（正样本预测为正样本，负样本预测为负样本）
   * F-measure = 2/(1/precision+1/recall)
      * F-measure，即F1，基于查准率与查全率的“调和平均”（(precision+recall)/2是算术平均，square_root(precision*recall)是几何平均）
 
