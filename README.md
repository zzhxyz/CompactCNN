A Compact Convolutional Neural Network for Textured Surface Anomaly Detection

Keras and PyTorch implementation of the CompactCNN. 

Details of the paper can be found [here](https://www.semanticscholar.org/paper/A-Compact-Convolutional-Neural-Network-for-Textured-Racki-Tomazevic/17d3f90cb63fbac50a5e49b8a46e633ec1f526fd#extracted).

Requirements:
keras,tensorflow,opencv,matplotlib,os,numpy

To run the code use `python ./ccnn_pytorch/main.py` or `python ./ccnn_keras/main.py`

To create DAGM dataset in the form required for this repository run the following command.

`python DAGM_data_prep.py "dataset directory path where you want the folders to be created" "DAGM folder path"`

For example:  `python DAGM_data_prep.py "/john/doe/datasets" "john/doe/DAGM"`

I've included the images folder in the repository as well the weights of the trained models.

Following is a sample result of the network.

![Sample Result](https://github.com/msminhas93/CompactCNN/blob/master/SampleOutput/output17.png)

The network outputs an anomaly heatmap and an anomaly score. The segmentation model is trained for 25 epochs and classification model for 10 epochs. However, the best model based on validation loss is kept. 
