# mnist_triplet_loss
Applying Triplet Loss function to MNIST dataset. Triplet loss maximizes distance between different classes and minimize distance between same classes. More about tensorflow's triplet loss implementation can be read [here](https://www.tensorflow.org/addons/tutorials/losses_triplet).
What this repo does:
- Load data from parquet and csv (the 28x28 pixels are flattened into one row)
- Make sure data have no problem
- Train embedding network (Triplet Loss applied here) and Base Network (Network to classify using softmax)
- Fit Base Network to embedding inferrenced pictures
- Calculate accuracy