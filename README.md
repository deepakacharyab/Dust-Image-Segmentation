# Identifying High-Latitude-Dust

TASK: Identify High Latitude Dust in a given MODIS imagery

**DATA FETCHING**

**DATA PREPROCESSING**

The dataset is small, so the following techniques can be used to preprocess the data before it is fed into the model. Image normalization is a typical process in image processing that changes the range of pixel intensity values between 0 and 255. The data is normalized by dividing the data by 255, which helps to bound the pixel intensity between 0 and 255. The other techniques involve image resizing, random cropping, horizontal and vertical flipping. The dataset is then split into training(80%) and validation set(20%). The data loader is then defined with training and validation set, and are then fed as input to the model.


**APPLYING ALGORITHM**

The U-net is a convolutional network architecture for fast and precise segmentation of images. I have used the U-net model to train and validate the test data. The train loader and validation loader are fed into the model to compute the loss and accuracy of the model. We have defined Binary Cross Entropy as a loss function, and the accuracy of the model is checked. There are different variants of the U-net model that can also be used for better results.


**EVALUATING THE MODEL**

The model performance is evaluated by plotting the Loss Vs. Epoch. The checkpoint is used to save the best performing model. The validation metrics F1 score, precision, recall, and accuracy are analyzed.


**VISUALIZING THE RESULTS**

The results are visualized from the model.


**EXECUTION**

Please use .ipynb file to run the execution. I get the details of the best model when I run Identifying_High_Altitude_Dust_Imagery.ipynb. Checkpoints folder has the saved model.
