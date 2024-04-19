# Object detection using deep learning algorithms: SSD and Faster RCNN

The final purpose of this project was to implement, adjust and train state of the art models on traffic-like images.

A comparison between Faster R-CNN (Faster Region-based Convolutional Neural Networks) and SSD (Single Shot Detector) trained 
for object detection tasks, using supervised learning as a training method and different tunning algorithms for constant 
improvement were applied on this project. Having these models trained in such a way, the resulTs were investigated for each 
network having as an input traffic-related objects within images (cars, traffic signs and pedestrians).

The Udacity self-driving dataset was chosen for training SSD and Faster RCNN models. The number of images in the beginning was 
around 30000. The dataset was divided in 127900 cars, 7194 trucks, 21491 pedestrians, 3704 bikers and many classes for traffic 
lights (13673 trafficLightRed, 3482 trafficLightRed-left, 541 trafficLightYellow, 28 trafficLightYellow-left, 10838 trafficLightGreen 
and 5101 under the name trafficLight). The dataset contains many classes which were in our interest but, at a first look, 
the problem of class imbalance was present. The class imbalance was solved using various ways, the final dataset countained 
69990 cars, 34277 traffic lights and 21491 pedestrians in 9533 images.

Each model was trained for about 80 epochs and was modified during training or started from scratch with a new perspective. 
As it was clear even while training, Faster RCNN outperformed SSD. That was a result that was expected because of its more 
complex architecture and due to its region proposal network that takes care of the proposals and their filtering.

The full paper, containg each step including the data preprocessing, tunning of parameters and the results is available in the
documentation section.
