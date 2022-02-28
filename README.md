# Master-degree-thesis-2015-UESTC
论文题目：基于高斯混合模型的EM算法及其应用研究

>电子科技大学, 硕士论文, 2015.
>
>https://kns.cnki.net/kcms/detail/detail.aspx?dbcode=CMFD&dbname=CMFD201601&filename=1015711236.nh&uniplatform=NZKPT&v=wAwkGweZ23URuizOOQpeSFOQB9QvquC4UZxiC0t_znSRbRS06vNfIchJdV7uu8ly

摘要： 高斯混合模型（GMM）被广泛应用于模式识别、计算机视觉、机器学习、数据挖掘、生物信息学等不同领域。 在这些领域里，它被用来完成诸如图像分割、聚类、概率密度函数的构建等任务。
    通常，人们用期望最大化（EM）算法求解GMM模型中的参数。尽管EM是一种非常有效的算法，且能保证收敛。但EM算法存在两个还没有被完全解决的问题：（1）因为EM只能保证收敛到局部最优点，所以EM算法对初始条件非常敏感；（2）用户需要预先设置GMM中高斯成员的个数，而在没有任何先验信息的情况下，如何设置高斯成员的个数也通常非常棘手。
    本文主要研究内容分为以下两个部分：
    在第一部分中，本文试图解决EM算法存在的不足。本文首先分析并指出EM算法的初始化敏感问题源于它的并行式学习策略所带来的高斯成员之间的竞争关系对公平的竞争条件的苛刻要求。由此，本文从改善学习策略的角度，在EM算法的前端加入了类似于EM算法的串行式学习过程，即让所有高斯成员在参与竞争前先避免竞争，以减小EM算法对随机初始条件的敏感程度。在串行学习阶段，所有的高斯成员都试图找到各自的散点簇，在参与竞争前先获得公平的竞争条件；在并行学习阶段，EM算法对串行学习的结果进行微调，通过高斯成员间的竞争式学习，获得全局最优的竞争结果。此外，用户也不用提前为设置高斯成员的个数。本文将所求解的GMM模型应用于聚类，结果表明本文的算法大大提升了EM算法在聚类应用上的性能。
    在第二部分中，本文试图继承EM算法的优点，以期获得一个更一般的学习模型，帮助人们解决不同领域的问题。首先，本文分析了EM算法的探索式学习本质，并从中抽象出了一种更一般的探索式学习模式。为了证明这种探索式学习模式在方法学层面上的有效性，本文随后又将这一探索式学习模式应用于循迹、知觉感知和轮廓检测这几个具体任务中，一定程度上证明了这一探索式学习模式是一种通用性的无监督的学习模式，可能具有广泛的应用价值。

**Abstract**: Gaussian mixture models (GMM) has been widely applied in diverse fields as pattern recognition, computer vision, machine learning, data mining, and bioinformatics, to complete diverse tasks as image segmentation, clustering, and function fitting. Expectation-Maximization (EM) algorithm is usually used to solve the parameters in GMM. Although EM algorithm is very effective and can guarantee the convergence, it has two open problems: (i) it is sensitive to initialization，since EM can only guarantee to converge to the local optimum; (ii) the number of Gaussian components in GMM needs to be specified in advance, whereas this number is usually hard to set without any prior information.
The contribution of this paper mainly contains two parts:
In the 1st part, we seek to solve the problems that EM algorithm has. This paper analyzed and pointed out that the initialization sensitivity problem for EM is largely due to that the competitive relationships among all Gaussian components, involved in the parallel learning process of EM algorithm, leads to the demanding requirement for the fair initial competition condition. Accordingly, from the perspective of strategy, a serial learning process, similar to EM algorithm, is added ahead of EM algorithm, that is, the competition should be avoided before the fair competition condition is obtained. In this way, influence of random initialization to EM can be largely reduced. In the serial learning phase, all Gaussian components try to fit with their own clusters, so as to create a fair competition condition; in the parallel learning phase, EM is used to fine-tune the above serial learning result, so as to reach a global optimum. Moreover, the number of Gaussian components in GMM doesn’t need to be specified in advance. Based on the proposed method, GMM model was then applied to cluster analysis. The result demonstrated that the proposed method largely improves the clustering performance of EM. 
In the 2nd part, we seek to inherit the merit of EM, in order to provide a more general learning model to help people solve problems in diverse fields. Firstly, this paper pointed out that EM is in nature a heuristic learning process, and extracted from EM a general heuristic learning model. In order to demonstrate its effectiveness, this learning mode was then applied to several specific tasks as tracking, perceptual organization and contour detection, which to some degree demonstrated this learning model can be a general unsupervised learning model and can be of general meaning.

# Code: in preparation...
# Figures （demos for the principle）

![image](https://github.com/Teng-Qiu-Clustering/Master-degree-thesis-2015-UESTC/blob/main/dynamic_fig.gif)


 
![image](https://github.com/Teng-Qiu-Clustering/Master-degree-thesis-2015-UESTC/blob/main/dynamic_fig_new.gif)
