# CV
## Paper
### AutoAugment: Learning Augmentation Policies from Data
Ekin D. Cubuk, Barret Zoph, Dandelion Mane, Vijay Vasudevan, Quoc V. Le
Google
Submitted on 24 May 2018
Paper: https://arxiv.org/abs/1805.09501
Code: https://github.com/tensorflow/models/tree/master/research/autoaugment
Comments: First paper in the field, same idea as AutoML: using RL to search the augmentation policy. Potential gains are shown, however, the main problem is the computation burden.

### RandAugment: Practical automated data augmentation with a reduced search space
Ekin D. Cubuk, Barret Zoph, Jonathon Shlens, Quoc V. Le
Google
Submitted on 30 Sep 2019
Paper: https://arxiv.org/abs/1909.13719
Code: https://github.com/tensorflow/tpu/blob/master/models/official/efficientnet/autoaugment.py
Comments: The main contribution is the reduced search space. Only two parameters left: N and M. (N: Number of augmentation transformations to apply sequentially; M: Magnitude for all the transformations)

### AugMix: A Simple Data Processing Method to Improve Robustness and Uncertainty
Dan Hendrycks, Norman Mu, Ekin D. Cubuk, Barret Zoph, Justin Gilmer, Balaji Lakshminarayanan
Google
Submitted on 5 Dec 2019
Paper: https://arxiv.org/abs/1912.02781
Code: https://github.com/google-research/augmix
Comments: Less severe augmentation policies and JS diversity loss are applied.
Questions: What's the sepearte effect for less severe policy and JS diversity loss? Is it benificial for clean data rather than corrupted datasets?

## Libraries
### imgaug
https://github.com/aleju/imgaug

This python library helps you with augmenting images for your machine learning projects. It converts a set of input images into a new, much larger set of slightly altered images.


# ASR
TBA
# NLP
TBA
# Pull requsts are welcome!
