# ViT and DeiT on Unconstrained Ear Recognition
##### A mini-project in EE298Z - Deep Learning, Semester 01 - 2020-2021
##### Coded and Performed by Marwin B. Alejo | 2020-20221 | University of the Philippines Diliman

##### Disclaimer:
This mini-project was planned originally to be executed on Detection-Transformer (DeTr). However due to the incompatibility of the ear recognition task with DeTr architecture and its complexity, this project was executed in Vision-Transformer and Data-effecient image Transformer (DeiT) instead. Furthermore, this is an extension of my 2019 study about Unconstrained Ear Recognition.

### Abstract
This mini-project extends Transformer Networks, Vision-Transformer (ViT) and Data-efficient image Transformers (DeiT) to be specific, to the Unconstrained Ear Recognition Task using the first 20 classes of EarVN1.0 [8] on Google Colab TPU node for ViT and GPU node on DeiT. The ViT model achieved a validation accuracy of 95% @ 20 epochs while 88.33% to 96.11 @ 20-50 epochs. These results are closely comparable with the CNN-based accuracy results of SOTA architectures through transfer learning and these architectures may practically be used as an alternative for an end-to-end development of an ear recognition system. The complete colaboratory notebook of this project may be accessed [here](https://github.com/soymarwin/ee298z/blob/main/Vision-Transformer%20on%20Unconstrained%20Ear%20Recognition%20-%20Marwin%20Alejo/Alejo_Marwin_ViT_Ear1.ipynb) or [directly in my drive](https://colab.research.google.com/drive/1Hg0isccTRi39FBfXJx9oS7nnUbumZHk2?usp=sharing) and the compiled PDF report [here](https://github.com/soymarwin/ee298z/blob/main/Vision-Transformer%20on%20Unconstrained%20Ear%20Recognition%20-%20Marwin%20Alejo/Alejo_Marwin_202020221_MiniProject_EE298Z.pdf)

### Resources
1. Google Colab TPU (Free node only)
2. PyTorch with XLA (ViT only)
3. Pretrained models on ImageNet may be found [here](https://github.com/rwightman/pytorch-image-models/releases/tag/v0.1-vitjx) for ViT and [here](https://github.com/facebookresearch/deit) for DeiT.
4. Trained models may be downloaded [here](https://drive.google.com/drive/folders/17P2o6bYQDBsP_FGbd51A1APzXpLT0d3H?usp=sharing) for ViT and DeiT.
5. EarVN1.0 dataset may be downloaded [here](https://data.mendeley.com/datasets/yws3v3mwx3/4). For this mini-project, only the first 20 folders are used with each images are splitted into 80:20 ratio.
6. My 2019 Unconstrained Ear Recognition study may be viewed [here](https://www.ijrte.org/wp-content/uploads/papers/v8i2/B2865078219.pdf) which I used for performance comparison with ViT and DeiT results.

### TODOs (for future explorers and hobbyists)
1. Generation of Tile Predictions (regardless of domain).
2. End-to-End combination of DeTr and ViT for a wide-scene multiple human imagery with detection and ear recognition.

### References
[1] Ž. Emeršič, V. Štruc and P. Peer, "Ear Recognition: More Than a Survey," CoRR, vol. abs/1611.06203, 2016.
<br>[2] Ž. Emeršič, D. Štepec, V. Štruc and P. Peer, "Training Convolutional Neural Networks with Limited Training Data for Ear Recognition in the Wild," in IEEE International Conference on Automatic Face & Gesture Recognition (FG 2017), Washington, DC, 2017.
<br>[3] E. Z. e. Al., "The Unconstrained Ear Recognition Challenge 2019," CoRR, 2019.
<br>[4] M. Alejo and C. P. Hate, "Unconstrained Ear Recognition through Domain Adaptive Deep Learning Models of Convolutional Neural Network," International Journal or Recent Technology and Engineering, vol. 8, no. 2, pp. 3143-3150, 2019.
<br>[5] N. Carion, F. Massa, G. Synnaeve, N. Usunier, A. Kirillov and S. Zagoruyko, "End-to-End Object Detection with Transformers," Lecture Notes in Computer Science, p. 213–229, May 2020.
<br>[6] A. Dosovitskiy, L. Beyer, A. Kolesnikov, D. Weissenborn, X. Zhai, T. Unterthiner, M. Dehghani, M. Minderer, G. Heigold, S. Gelly, J. Uszkoreit and N. Houlsby, "An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale," CoRR, October 2020.
<br>[7] M. C. Hugo Touvron, M. Douze, F. Massa, A. Sablayrolles and H. Jégou, "Training data-efficient image transformers & distillation through attention," CoRR, December 2020.
<br>[8] V. T. Hoang, "EarVN1.0: A new large-scale ear images dataset in the wild," Data in Brief, vol. 27, 2019.

