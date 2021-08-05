# Vehicle_Classification_model
A model to classify bus/car/2wheeler based on keras and 10 layered neural network

We start with preprocessing of the data provided.We are using Keras ImageDataDenerator to preprocess.
We split our data into train and Test using IDG(validation_split=0.2) marking 20% of our data as validation data.
In preprocessing , we converted or data into GRAYSCALE for faster training and created batches of 128 each.
We reduced the size of data into 48*48 pixels. 

After preprocessing we made Sequential model from Keras and created deep Neural network of 10 layers.
Starting with:
1. Convolutional 2D layer
2. Relu Actication
3. Convolutional 2D
4. Relu Actication
5. Maxpool
6. Dropout 
7. Flatten
8. Dense
9. Relu Actication
10.Dropout
And Final Dense converting entire Tensor into a 3 class based layer.
We ran 10 epochs and saved the model with best accuracy into a .h5 file.

