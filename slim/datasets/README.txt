# This folder is for processing the training data

# Below is the description of some important files in the folder

######################################### 


# convert_eye.py: file used to change jpeg images into the TFRecord format. It splits the total dataset into two sub datasets: train and validation. The size of the validation set is set to 7030 by default. For each sub dataset, there are five equal-number shards, which consists of images from different classes(0,1,2,3,4)

usage: 
1 change directory to slim
2 open python shell 
'''python
import datasets.convert_eye as convert
dataset_dir='./DR_data'
convert.run(dataset_dir)
'''



# eyes.py: file used to change TFRecords into slim dataset format, which is then used as input data for training. It sets the size of training samples as 21075, validation samples as 14051(6:4). We don't have test set here.

 
