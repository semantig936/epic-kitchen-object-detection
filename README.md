# epic-kitchen-object-detection
OpenCV `dnn` module supports running inference on pre-trained deep learning models from popular frameworks like Caffe, Torch and TensorFlow. It is used to detect spoon or knife from the epic kitchen data set

When it comes to object detection, popular detection frameworks are
 * YOLO
 * SSD
 * Faster R-CNN
 
 Support for running YOLO/DarkNet has been added to OpenCV dnn module recently. 
 
 ## Dependencies
  * opencv
  * numpy

## YOLO (You Only Look Once)
Download the pre-trained YOLO v3 weights file from this [link](https://pjreddie.com/media/files/yolov3.weights) and place it in the current directory or you can directly download to the current directory in terminal using
 
 `$ wget https://pjreddie.com/media/files/yolov3.weights`
It cannot be pushed to github
## Epic Kitchen
Epic kitchen data set: https://epic-kitchens.github.io/2024

## To run the program

considering the image and weight file in the same directory

`$ python3 yolo_opencv.py --image spoon-group.jpeg --config yolov3.cfg --weights yolov3.weights --classes yolov3.txt`