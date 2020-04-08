# CV
## Paper
### AutoAugment: Learning Augmentation Policies from Data
Ekin D. Cubuk, Barret Zoph, Dandelion Mane, Vijay Vasudevan, Quoc V. Le  
Google  
Submitted on 24 May 2018  
Paper: https://arxiv.org/abs/1805.09501  
Code: https://github.com/tensorflow/models/tree/master/research/autoaugment  
Comments: 该领域的第一篇文章，和AutoML的思路一样：使用强化学习来搜索数据增强策略。结果显示还是有收益的，但主要的问题是计算量太大（每一个策略都要训练一遍才知道效果如何）。

### RandAugment: Practical automated data augmentation with a reduced search space
Ekin D. Cubuk, Barret Zoph, Jonathon Shlens, Quoc V. Le  
Google  
Submitted on 30 Sep 2019  
Paper: https://arxiv.org/abs/1909.13719  
Code: https://github.com/tensorflow/tpu/blob/master/models/official/efficientnet/autoaugment.py  
Comments: 主要贡献是减小了搜索空间，只剩下了N和M两个参数。(N: 增强变换串联的次数; M: 所有增强变换相同的幅度)

### AugMix: A Simple Data Processing Method to Improve Robustness and Uncertainty
Dan Hendrycks, Norman Mu, Ekin D. Cubuk, Barret Zoph, Justin Gilmer, Balaji Lakshminarayanan  
Google  
Submitted on 5 Dec 2019  
Paper: https://arxiv.org/abs/1912.02781  
Code: https://github.com/google-research/augmix  
Comments: 使用了和原始数据接近的增强方式，另外在loss函数中增加了JS diversity来牵引网络对不同的增强变换保持鲁棒。  
Questions: 上面提到的两种手段对最终效果的贡献分别是多少？对CIFAR-10/100, ImageNet这种原始数据集，而不是CIFAR-10-C/100-C, ImageNet-C这些数据集有无收益？

### SuperMix: Supervising the Mixing Data Augmentation
Ali Dabouei, Sobhan Soleymani, Fariborz Taherkhani, Nasser M. Nasrabadi  
West Virginia University  
Submitted on 10 Mar 2020  
Papaer: https://arxiv.org/abs/2003.05034
Code: https://github.com/alldbi/SuperMix  
Comments: 使用了teacher network来指导mask的生成，相对于CutMix等更有针对性。SuperMix 的优化目标有三个：i) 输入图像的类别出现在混合后的图像中；ii)保留图像的局部结构；iii) 降低抑制重要特征的风险。  

## Libraries
### imgaug
https://github.com/aleju/imgaug

This python library helps you with augmenting images for your machine learning projects. It converts a set of input images into a new, much larger set of slightly altered images.


# ASR
TBA
# NLP
TBA
# Pull requsts are welcome!
