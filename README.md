# MLND-p2-submit
# 2018-7-1 Review
这个题目比较主观，GBDT模型的优缺点你可以根据自己的理解来，例如优点可以是：
off-the-shelf方法，工业上大量应用，几乎所有问题都可以直接用GBDT。现在的GBDT可以高效的进行数据并行（如XGBoost，LightGBM等），适合处理超大规模数据，相比绝大多数模型，训练准确性高；鲁棒性高，通常对outlier不敏感；可以输出特征重要性。 等等
同样缺点也有：
不能进行批训练或者增量训练；高维稀疏特征下不如LR的泛化能力好，比如CTR预估等场景中

你可以参考这个知乎文章，从看Tree Boost方法的讲解（包括Adaboost和GBDT)。另外我更推荐一个从应用角度更形象的解释，参见Kaggle.
。。。
这里最好引出GBDT中残差的概念。以及你需要理解GBDT中的Gradient是针对什么的Gradient。
HINT：GBDT的一个优点是可以优化任何可微的损失函数，请思考这个是为什么？你可以在模型对比的批注部分，在给出的两个链接中找到答案。为此，你可能需要仔细阅读一下这两篇文章。
