# EE298Z-Assignment01
##### Written and performed by Marwin B. Alejo 2020-20221

### Requirements
1. Build a classifier on CIFAR10 dataset using MLP and CNN
2. The last layer is Dense
3. Hyperparameters are tweakable but optimizer remains SGD
4. Show solution using Jupyter notebook and shared via github
5. Implement using Keras or Pytorch
6. Compare performance of best MLP and CNN

### Used Compute Resources
1. Google Colab CPU(MLP only) and TPU(both MLP and CNN)

## Overall Summary of Results
After several trials of network configuration design while considering the above-listed requirements, the following configurations are found to be the best performing MLP and CNN. Link to the best performing MLP and CNN configurations can be found [here](https://github.com/soymarwin/ee298z-assignment01/blob/master/best_mlp_cnn_cifar10.ipynb).<br>
<br> Cifar10 classifier on 3-layer MLP (Accuracy: 53.49%):
<br>
![alt text](https://github.com/soymarwin/ee298z-assignment01/blob/master/best_mlp_acc_53.png)
<br>
![alt text](https://github.com/soymarwin/ee298z-assignment01/blob/master/best_mlp_loss_53.png)
<br>
<br> Cifar10 classifier on 3-layer CNN (Accuracy: 82.85%):
<br>
![alt text](https://github.com/soymarwin/ee298z-assignment01/blob/master/best_cnn_acc_82.png)
<br>
![alt text](https://github.com/soymarwin/ee298z-assignment01/blob/master/best_cnn_loss_82.png)
<br>
<br> Cifar10 classifier on 3-block CNN (Accuracy: 89.17%):
<br>
![alt text](https://github.com/soymarwin/ee298z-assignment01/blob/master/best_cnn_acc_89_.png)
<br>
![alt text](https://github.com/soymarwin/ee298z-assignment01/blob/master/best_cnn_loss_89_.png)
<br>

<br> The best performing MLP from the pool of MLP trials achieved an accuracy score of 53.49%. Although other MLP configurations achieved a test accuracy of more than 55%, it is observed that these configurations are overfitting.

<br> Likewise, the best performing 3-layer CNN from the pool of CNN trials achieved a test accuracy of 82.85%. The unique parameter in this configuration is that it uses the LeakyReLU activation function as configurations with eLU and ReLU yields lower accuracies.

<br> Additionally, a 3-block CNN was explored and yields a test accuracy of 89.17%. Unlike the 3-layer CNN configuration above, this 3-block CNN uses the eLU activation function and average pooling.

<br> Overall, in terms of performance, eventhough CNN is computationally expensive in comparison to MLP, CNN performs better for image classification task than MLP. Although MLP is capable of the said task, it is prone to abnormal(under/over) fitting depending on the extent of the MLP network design. Also, with the 3-layer network design requirement, CNN achieves an accuracy of 82% to 89% while MLP achieves at arounf 52% to 56%. 

<br> Complete trials and other MLP and CNN configurations may be found [here](https://github.com/soymarwin/ee298z-assignment01/blob/master/complete_cifar10_mlp_cnn_trials.ipynb) or in this [colab notebook](https://colab.research.google.com/drive/1XjdwCKeoqJzHGCn1kadpF2urVXlkwDcH?usp=sharing).