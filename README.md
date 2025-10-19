# PV-ChangeNet
The offical implementation of detecting Photovoltaic expansion in farmland: A progressive difference amplification change detection network and a change detection dataset

# Requirement
* ubuntu 18.04 <br>
* python 3.8<br>
* pytorch 1.10<br>

# Dataset
The dataset should consist of pairs of images(before and after) in TIFF format, with each pair containing: A.tif and B.tif for the before and after images, respectively. label.tif for the ground truth(binary mask indicating change or no-change).

The dataset is avaliable at: https://pan.baidu.com/s/1FsIfdmo4UZN500vVdGXGYw?pwd=1234

# Working Example
Training the Model.
(1) Prepare the Dataset. Make sure your dataset is structured as described above and adjust the dataset_path variable in the training script to point to your training data folder. (2) Training Script. To train the PV-ChangeNet model, run the following command:
···
pthon train.py
···
Testing the Model.
(1) Prepare the Dataset. Make sure your dataset is structured as described above and adjust the dataset_path variable in the testing script to point to your testing data folder. (2) Testing Script. To test the trained model on the test dataset, run the following command:
···
pthon test.py
···
# Acknowledgments
The sample data that support the findings of this study are available at 10.1016/j.rse.2024.114100
