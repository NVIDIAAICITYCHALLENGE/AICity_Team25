# AICity_Team25

We participated in the Track 1 of Nvidia's AICITY Challenge and our goal was to train a model using any framework and detection algorithm.
To achieve this, we have used caffe framework with Detectnet as well as Darknet with Yolo. The models generated by using both of these techniques
are in the folders 'Detectnet' and 'Yolo' respectively. The folders contain the codes for each of these techniques as well.

The model generated using Detectnet has to be imported into Digits and can be tested using any image. The DIGITS GUI is easy to use and self explanatory.

The model generated usng Darknet and Yolo can be tested on images as well as videos. The weights file is named as yolo-aic_30000.weights
which is located inside the 'Yolo' folder. 

First Darknet needs to be cloned from https://github.com/pjreddie/darknet and has to be installed. Copy the yolo-aic.data and yolo-aic.cfg into 
the '/darknet/cfg/' folder.

Command to test the model using an image is:

./darknet detector test cfg/yolo-aic.data cfg/yolo-aic.cfg yolo-aic_30000.weights 'path to the image to be tested'

Command to test the model using a video is:

./darknet detector demo cfg/yolo-aic.data cfg/yolo-aic.cfg yolo-aic_30000.weights 'path to the video to be tested'

Our model generated with Darknet and YOLO has a Mean Average Precision (mAP) of 0.31 and it's ranks fourth amongst all the teams. 

