>典故：公元前1202年，意大利数学家列昂纳多.斐波拉契在《算盘全书》中描述了一个兔子序列，这就是著名的斐波拉契序列
>假设第一个月诞生一对兔子，第二个月进入成熟期，第三个月开始生育兔子，假设一对成熟的兔子每月会诞生一对兔子，
>兔子永不死去，那么按照这个理论，12个月有多少对兔子?

1. 概述

    动态规划也是一种分治思想，但是与分治算法不同的是，分治算法是吧原问题分解为若干子问题，然后自顶向下求解各个子问题，合并子问题的解，从而得到原问题的解。动态规划也吧原问题分解为若干子问题，然后自底向上，先求解最小的子问题，把结果存储在表格中，在求解大的子问题时，直接从表格中查询小的子问题的解，避免重复计算，从而提高算法的效率。
2. 算法要素

    两个性质：
    * 最优子结构
        最优子结构性质是指问题的最优解包含其子问题的最优解。自由子结构是使用动态规划的最基本的条件，如果不具有最优子结构性质，就不可以使用动态规划解决。
    * 子问题重叠问题
        子问题重叠是指在求解子问题的过程中，有大量的子问题时重复的，那么只需要求解一次，然后把结果存储在表中，以后使用时可以直接查询，不需要再次求解。子问题重叠不是使用动态规划的必要条件，大事问题存在子问题重叠更能充分彰显动态规划的优势。


3. 动态规划秘籍
    1. 分析最优解的结构特征
    2. 建立最优值得递归式
    3. 自底向上计算最优值，并记录
    4. 构造最优解
4. 实战演练
    1. [兔子序列问题]()