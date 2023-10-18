# Music-Genre-Classification

In this project, I have downloaded all the necessary files through the !wget method. Then after extracting, I converted all the files to .wav format (originally they were .au). 
Next I created a JSON file containing the class mappings (i.e 'classical', 'rock', etc), labels for the respective mappings and the mfcc features. Each of the audio file in each genre has been split into segments and the MFCC's have been calculated for each segment. 
Then, I created test and validation sets with 25% and 20% of the data respectively. The X_train, X_test and X_validation are reshaped to suit the CNN architecture. Finally, I built the 2D-CNN (input data excludes the batch size). The activation functions are standard 'RELU' and 'SoftMax'. I got validation accuracy as 75% on my first run.
The model also correctly predicted the labels for randomly selected files from test dataset. 
