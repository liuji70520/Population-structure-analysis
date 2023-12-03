# 群体结构分析指南

## 1、群体结构分析的概念和重要性                                 
### 群体结构的定义
又称群体分层，指所研究的群体中存在基因频率不同的亚群。
比如我们研究一种在东南亚的沙梨，通过PCA等方法把中国和朝鲜半岛与日本的沙梨分为三个亚群。（T：这三个亚群就是群体结构）
### 群体结构分析的目的和应用
群体结构分析最突出的一点是它能够通过主成分分析（PCA）（T:principal component analysis）、系统进化树、structure等方法，反映遗传变异在物种或群体的分布，推断群体数目，判断某个体属于哪个群体。这种分析能够提供个体的血统来源及其组成信息，是一种重要的遗传关系分析手段。


（计划高亮分行处理）	举例：假设我们正在研究一种沙梨。这种沙梨分布在中国、朝鲜半岛和日本。我们想要了解这些群体之间的遗传差异，以及它们是否形成了不同的亚种。
首先，我们可以收集来自不同地理位置的沙梨样本，然后提取它们的DNA。通过测序，我们可以得到每个样本的基因组信息。
然后，我们可以使用主成分分析（PCA）等统计方法，根据这些基因组信息来分析沙梨群体体的结构。PCA可以帮助我们理解基因变异在不同群体中的分布情况，从而推断出可能存在的亚种。
最后，我们可以根据PCA的结果，将沙梨样本分为不同的群体，每个群体代表一个可能的亚种。

![xi](https://media.springernature.com/lw685/springer-static/image/art%3A10.1038%2Fs41467-021-21378-y/MediaObjects/41467_2021_21378_Fig1_HTML.png?as=webp)

Phylogenetic relationship and population structure of 312 sand pears. a Phylogenetic tree of sand pears. b Population structure of sand pears. K value is 2. c PCA of sand pears. Group I with red background corresponds to the Chinese group, and Group II with blue background indicates the Japanese and Korea group.

PCA：运用方差分解，将海量SNP的差异反映在二维坐标图上，坐标轴轴取对样品差异性解释度最高的两个或三个特征值，样本SNP位点信息越相似，反映在PCA图中的距离越近
## 2. 群体结构分析的方法
这里主要讲Structure。其原理是将群体分成 K 个服从 Hardy-Weinberger(HWE) 平衡的亚群，每个材料归到各个亚群，计算每个材料其基因组变异源于第 K 个亚群的可能性(Pritchard et al.2000)，主要用 Q 矩阵表示，Q 值越大，表明某个材料来自某个亚群的可能性越大。



## 3. 群体结构分析的步骤
🪗软件准备
[Structure官网下载](https://web.stanford.edu/group/pritchardlab/structure_software/release_versions/v2.3.4/html/structure.html)

☕数据准备
[.vcf文件格式解读（内含其他各种生信常见格式解读）](https://learn.gencore.bio.nyu.edu/ngs-file-formats/vcf-format/)

[本次所用.vcf数据下载链接](https://www.ncbi.nlm.nih.gov/tools/gbench/tutorial8/)

[Structure详细教程](https://zhuanlan.zhihu.com/p/383141001)



vcf格式解读：[.vcf](https://learn.gencore.bio.nyu.edu/ngs-file-formats/vcf-format)
## 参考文献
[Genome-wide association studies provide insights into the genetic determination of fruit traits of pear](https://doi.org/10.1038/s41467-021-21378-y)
