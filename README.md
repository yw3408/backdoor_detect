# Backdoor Detection and Cleanse

## Group Member

Yunrui Huang(yh2910)



## Evironment



## To run 

To run `Fine_Pruning_Weight_Pruning.ipynb`, please modify the  

Please put the validation and test datasets under "/content/drive/MLsecurity_project/data/" directory.
Also, please put model files under "/content/drive/MLsecurity_project/models/" directory.

## Instruction for running the Entropy filter notebook:

First put all the data.h files under the path below:
"/content/drive/MyDrive/MLsecurity_project/data/"
And also put all the model.h files under the path below:
"/content/drive/MyDrive/MLsecurity_project/models/"
Then, you could just run the whole notebook. 
If you want to use your own test data, just replace the input data on this three parts:
Model repair->For sunglasses_bd_net.h5->Input data
Model repair->For multi_trigger_multi_target_bd_net.h5->Input data
Model repair->anonymous_bd_net.h5->Input data

