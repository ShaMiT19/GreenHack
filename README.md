# GreenHack
The topic we chose for this Hackathon was Transmission system Operator of the future.
In this we were expected to make a machine learning model which would detect the electrical masts and classify them accordingly.

For this task we were also provided with a few drone images of electrical masts. 

There are basically 2 types of machine learning models: supervised and unsupervised models. 
Since we had to classify the electrical masts we decided to go with supervised models, for this we needed labeled data. 
There are a lot of supervised deep learning algorithms which could have been used for solving this problem, but we chose to go with masked rcnn.

Starting with our work,
The first step for us was to create a labelled data for the deep learning model. We created this labelled data by marking the electrical masts on makesense.ai which exports these labelled data in JSON form. 

Then we used the Masked RCNN github repository and created our model. Our model has two main files named as custom.py and predict.py.
The custom.py is used for training the dataset and predict.py is used for prediction of the electrical mast on any given image. 

For the training and testing of model we used google colab, we first mounted our google drive on google colab and started training the model using the custom.py file. Due to lack of computational power we could not completely train the model. Provided more data and time both the efficiency and accuracy of our model  are sure to increase.

The output of our model would look something like this marking the outline of electrical mast.

Presentation Link for this project : https://www.youtube.com/watch?v=NHjlce2cNF0&list=LL&index=35
