# Vision-Transformer on Unconstrained Ear Recognition
##### A mini-project in EE298Z - Deep Learning, Semester 01 - 2020-2021
##### Coded and Performed by Marwin B. Alejo | 2020-20221 | University of the Philippines Diliman

##### Disclaimer:
This mini-project was planned originally to be executed on Detection-Transformer (DeTr). However due to the incompatibility of the ear recognition task with DeTr architecture and its complexity, this project was executed in Vision-Transformer instead, a Transformer network for any recognition task. Furthermore, this is an extension of my 2019 study about Unconstrained Ear Recognition.

### Abstract
This mini-project extends Transformer Networks, Vision-Transformer (ViT) to be specific, to the Unconstrained Ear Recognition Task using the first 20 classes of EarVN1.0 [7] on Google Colab TPU node. The model achieves a validation accuracy of 95% and is closly comparable with the CNN-based accuracy results of SOTA architectures through transfer learning. Complete colaboratory notebook maybe accessed [here](https://github.com/soymarwin/ee298z/blob/main/mini-project/Alejo_Marwin_ViT_Ear1.ipynb) or [directly to my colab notebook here](https://colab.research.google.com/drive/1Hg0isccTRi39FBfXJx9oS7nnUbumZHk2?usp=sharing) and the compiled report in PDF [here](https://github.com/soymarwin/ee298z/blob/main/mini-project/Alejo_Marwin_202020221_MiniProject_EE298Z.pdf)

### Resources
1. Google Colab TPU (Free node only!)
2. PyTorch with XLA
3. Pretrained models on ImageNet may be found [here](https://github.com/rwightman/pytorch-image-models/releases/tag/v0.1-vitjx) for those who would want to extend this project.
4. 95% trained model may be downloaded [here](https://drive.google.com/drive/folders/17P2o6bYQDBsP_FGbd51A1APzXpLT0d3H?usp=sharing).
5. EarVN1.0 may be downloaded [here](https://data.mendeley.com/datasets/yws3v3mwx3/4)
6. My 2019 Unconstrained Ear Recognition study may be viewed [here](https://www.ijrte.org/wp-content/uploads/papers/v8i2/B2865078219.pdf)

### TODOs (for future explorers)
1. Generation of Tile Predictions (regardless of domain).
2. End-to-End combination of DeTr and ViT for a wide-scene multiple human imagery with detection and ear recognition.

### References
1. Ž. Emeršič, V. Štruc and P. Peer, "Ear Recognition: More Than a Survey," CoRR, vol. abs/1611.06203, 2016.
2. Ž. Emeršič, D. Štepec, V. Štruc and P. Peer, "Training Convolutional Neural Networks with Limited Training Data for Ear Recognition in the Wild," in IEEE International Conference on Automatic Face & Gesture Recognition (FG 2017), Washington, DC, 2017.
3. E. Z. e. Al., "The Unconstrained Ear Recognition Challenge 2019," CoRR, 2019.
4. M. Alejo and C. P. Hate, "Unconstrained Ear Recognition through Domain Adaptive Deep Learning Models of Convolutional Neural Network," International Journal or Recent Technology and Engineering, vol. 8, no. 2, pp. 3143-3150, 2019.
5. N. Carion, F. Massa, G. Synnaeve, N. Usunier, A. Kirillov and S. Zagoruyko, "End-to-End Object Detection with Transformers," Lecture Notes in Computer Science, p. 213–229, May 2020.
6. A. Dosovitskiy, L. Beyer, A. Kolesnikov, D. Weissenborn, X. Zhai, T. Unterthiner, M. Dehghani, M. Minderer, G. Heigold, S. Gelly, J. Uszkoreit and N. Houlsby, "An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale," CoRR, October 2020.
7. V. T. Hoang, "EarVN1.0: A new large-scale ear images dataset in the wild," Data in Brief, vol. 27, 2019.
