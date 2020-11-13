# EE298Z-Assignment02
##### Performed by Marwin B. Alejo 2020-20221

### Requirements
1. Use autoeconder to build unsupervised classifier.
2. Use AE to train E
3. Use K-means
4. Use Hungarian algorithm

### Used Compute Resources
1. Google Colab TPU

### Time for training and evaluation (code and parameter modification is excluded)
~45 minutes in an ideal network speed and weather condition.

## Overall Summary of Results
Unsupervised classifier may be achieved using encoders as demonstrated in [this colab notebook](https://github.com/soymarwin/ee298z/blob/main/assignment02/EE298Z_Assignment02.ipynb) or [here](https://colab.research.google.com/drive/1pnHhlNW2IQ3TEJfo_rMdu1SWrDxu2gYu?usp=sharing). The best [configuration](https://colab.research.google.com/drive/1pnHhlNW2IQ3TEJfo_rMdu1SWrDxu2gYu?authuser=3#scrollTo=8T0kNuPIC5Fb&line=1&uniqifier=1) achieved an accuracy of ~96.00% as shown in figure below. Autoencoder training and clustering through K-means is provided in the provided notebooks above while autolabeling through Hungarian algorithm was implemented in a separate module ([see metrics.py](https://github.com/soymarwin/ee298z/blob/main/assignment02/metrics.py) or [here](https://drive.google.com/file/d/1vmBW6G2tlyhvUAFGuiGtBdjGKmy9olK7/view?usp=sharing)). Evaluations are provided in each configuration to assess each unsupervised models.
<br>
![alt text](https://github.com/soymarwin/ee298z/blob/main/assignment02/accuracy.jpg)