# ACRNN
Code for paper: EEG-based Emotion Recognition via Channel-wise Attention and Self Attention
## About the paper
* Title: [EEG-based Emotion Recognition via Channel-wise Attention and Self Attention](https://www.researchgate.net/publication/344281379_EEG-based_Emotion_Recognition_via_Channel-wise_Attention_and_Self_Attention)
* Authors: Wei Tao, Chang Li, Rencheng Song, Juan Cheng, Yu Liu, Feng Wan and Xun Chen
* Institution: Hefei University of Technology
* Published in: IEEE Transactions on Affective Computing
## Instructions
* Before running the code, please download the DEAP dataset, unzip it and place it into the right directory. The dataset can be found [here](http://www.eecs.qmul.ac.uk/mmv/datasets/deap/index.html). Each .mat data file contains the EEG signals and consponding labels of a subject. There are 2 arrays in the file: **data** and **labels**. The shape of **data** is (40, 40, 8064). The shape of **label** is (40,4). 
* Please run the deap_pre_process.py to Load the origin .mat data file and transform it into .pkl file.
* Using ACRNN.py to train and test the model (10-fold cross-validation), result of 10 folds will be saved in a .xls file.
* ACRNN.py is used to calculate the final accuracy of the model.
* The usage on DREAMER dataset is the same as above. The DREAMER dataset can be found [here](https://zenodo.org/record/546113/accessrequest). 
## Requirements
+ Pyhton3.5
+ tensorflow-gpu (1.4.1 version)

If you have any questions, please contact yc07466@umac.mo

## Reference
* [ynulonger/ijcnn](https://github.com/ynulonger/ijcnn)
