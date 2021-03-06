统计大坑列表
============
在收集特征之后需要进行真正的统计分析过程，这里列举了需要注意的问题

## 涉及内生性的问题
* 大多数人都是人云亦云，本身的态度是看完高赞答案后得出 **（存在未纳入统计的特征）**

这类随机干扰项的自相关，我们采取的方法是引用SDM模型，把其相关联的点赞和关注回答的用户找出来，再用他们的解释变量加进来做回归。

* 家庭背景可能导致他们的教育不同，但家庭背景又和这个倾向是有关的 **（非因果的相关性，存在未纳入统计的特征）**
* 越喜欢舆论造势的人越会参加这个讨论 **（样本自选择）**
* 越喜欢数学的人越会参加这个讨论 **（样本自选择）**
