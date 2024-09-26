I have Simplified the dataset by creating an AgeFolderDataset class which automatically retrieves the image path and labels based on the folder names. One of the challenges that I faced was the risk of overfitting. Beacuse the dataset is not that huge and ore complex architectures might not be favourable. I even implemented Hyperparameter tuning. I used optuna to do this. I set 50 different scenarios for hyperparameter tuning so that I can get the best result which will be optmizied to this particular CNN. Initially when I had set the learning rate at 0.001 and batch size 64, I was getting MSE > 5. After I implemented it, I achieved a MSE of 3.85 which is a good result taking teh dataset size and the model simplicity into picture. Please do Ignore the plotly error as I did not have it installed on my system.

a. Model Architecture:
I have created a CNN with
3 Convolution layers
max pooling layer
2 fully connected layers
This is a very simple CNN and I tried to focus on the model's ability of feature extraction and tried to keep it simple so that model does not behave in an unpredictiable way.

b. Classification Accuracy:
-I have used Mean Absolute Error to evaluate the model's performance. I achieved MSE = 3.85 which I think is pretty decent considering the dataset size and the simplicty of the model.

c. What worked well:
-The model was able to learn well with a reasonable validation loss and mean absolute error. The training in the initial epochs was a bit rough, but nearing 80+ epoch, it started to stabilize which meant that the model was able to learn well and overfitting is also not the case here.

d. What did not work well:
-F1 score was not working well and did not show the data that we could see and then come to a conclusion where the model might be going wrong and could make changes in the model. 

e. Improvement Suggestions
- Increasing the size of Dataset
- Use Transfer Learning with CNNs like Resnet or YOLO
- Increase the complexity of the model which will help to learn the features in more detail which will increase the accuracy of the model.

f. Using the provided Dataset to make a person look younger or older
- I think GANs would be the best fit here. 
- Collecting a dataset with more diverse features such as different background, skin tones, various ages, pictures with different angles.

I thank you for considering my application and giving me a chance to possibly work in you organization!

Best Regards, 
Nikhil Joshi
(+91)7702103173
