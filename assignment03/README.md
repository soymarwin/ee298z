# EE298Z-Assignment03
##### Performed by Marwin B. Alejo 2020-20221

### Requirements
1. Perform [AdaIN Style Transfer of Huang and Belongie](https://arxiv.org/abs/1703.06868) on SVHN (source style) and MNIST (target/content) datasets.

### Used Resources
1. Google Colab CPU for pre-processing and GPU for training and testing. (Free node only!)
2. PyTorch (100% Recommended framework for GAN and Tranformers)
3. [MNIST image-only testset](http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz), no need for labels). Preprocessed MNIST test set may be downloaded [here](https://drive.google.com/drive/folders/11plhHR7DPpYEZGEHrg6Rc5h1hUM2Ipm9?usp=sharing).
4. [SVHN cropped trainset](http://ufldl.stanford.edu/housenumbers/train_32x32.mat). Preprocessed SVHN  cropped train set may be downloaded [here](https://drive.google.com/drive/folders/12h7VfLTQNhgzOaeux2OP0D4mM-f1MRIk?usp=sharing)

### Process
1. Download both the SVHN and MNIST using wget command in Google Colab and place it on your desired Google Drive directory.
2. Extract images from the compressed imagesets into your desired Google Drive directory. This may be done by 

### Execution training time.

Disclaimer: Since Google Colab is the chosen platform in this assignment execution, training performance(speed) depends on your node of choice, plan, and internet connectivity. Better use Google Colab Pro or GCC node for a faster compute time and longer training time node allocation. Additionally, due to the said  compute constraint, only up to 20000 iteration is performed.

1. ~1 hour in an ideal network speed and weather condition for 500-1000 iterations.<br>
2. ~2 hours for 10000 iterations. <br>
3. ~4 hours for 20000 iterations. <br>

### Overall Observation
As demonstrated in [this colab notebook](https://github.com/soymarwin/ee298z/blob/main/assignment03/EE298Z_Assignment03.ipynb) or [here](https://colab.research.google.com/drive/1pnHhlNW2IQ3TEJfo_rMdu1SWrDxu2gYu?usp=sharing) using the python scripts above. The following styled images below are the product of generated weights per set iteration. Due to the compute resource limitation and time constraint, only the iterations below were performed however, theoretically, the longer the weights are trained, the better the styled image outcome would be regardless the content shape. In this case, SVHN is a 3 channel 32x32 imageset while MNIST is a 1 channel 28x28 imageset. The generated weights of this assignment are in the [model folder](https://github.com/soymarwin/ee298z/blob/main/assignment03/model). The [test.py](https://github.com/soymarwin/ee298z/blob/main/assignment03/test.py) in this execution was modified to to reshape mnist contents to (1,3,32,32) from (1,1,28,28) and match with the input of trained weight: (64,3,32,32).

Additionally, in comparison with SGAN and CycleGAN which are more on value transfer as shown in [here](https://github.com/yunjey/mnist-svhn-transfer), AdaIN Style Transfer is more on artistic transfer.
<br>
#### Sample Content (target) MNIST Input
![sample_target.png](https://github.com/soymarwin/ee298z/blob/main/assignment03/sample_target.png)
<br>
#### Sample Style SVHN Input
![sample_style.png](https://github.com/soymarwin/ee298z/blob/main/assignment03/sample_style.png)
<br>
#### Output from 500 iter weight
![9999_stylized_09999_iter500.png](https://github.com/soymarwin/ee298z/blob/main/assignment03/styled_images/9999_stylized_09999_iter500.png)
<br>
#### Output from 10000 iter weight
![30_stylized_00003_iter10000.png](https://github.com/soymarwin/ee298z/blob/main/assignment03/styled_images/30_stylized_00003_iter10000.png)
<br>
#### Output from 20000 iter weight
![30_stylized_00003_iter20000.png](https://github.com/soymarwin/ee298z/blob/main/assignment03/styled_images/30_stylized_00003_iter20000.png)
<br>

### TODO (for future explorers)
1. Unified preprocessing (environment preparation) on Google Colab.
2. Training using [extra set of SVHN cropped](http://ufldl.stanford.edu/housenumbers/extra_32x32.mat). 
3. Training and testing using PyTorch's in-house [MNIST and SVHN datasets](https://pytorch.org/docs/stable/torchvision/datasets.html).

### References
1. [Original paper of Huang and Belongie](https://arxiv.org/abs/1703.06868)
2. [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)
3. [AdaIN TF-K implemetation](https://github.com/ftokarev/tf-adain)
4. [AdaIN PyTorch implementation](https://github.com/naoto0804/pytorch-AdaIN)
5. [Basis: AdaIN PyTorch implementation](https://github.com/kukosmos/adain-pytorch-2019)