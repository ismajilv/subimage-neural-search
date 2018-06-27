# README #

Exploring the use of deep learning models for subimage search: given images A and B, is the object on image B also on image A. Presumably image A is much bigger than image B. The idea is to pass both images through pre-trained deep neural network (i.e. ResNet) to produce convolutional features for both (dense classification layers are discarded). Then convolve image B features over image A features to calculate the match score. The scores are used to predict the location of image B on image A. Global max pooling over all scores is used to predict existence of object B on image A. We coded the model, come up with evaluation metrics and experiment with different layers etc. 

VGG16 pre trained model is used. 
