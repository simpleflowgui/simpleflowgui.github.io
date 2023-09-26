# Nodes Guide

## Basic Library

<a href="alternative text"><img src="https://raw.githubusercontent.com/simpleflowgui/simpleflowgui.github.io/main/imgs/basiclib.png" align="middle" width="200" height="100"></a>


### Start Node: 

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/startn.png" align="middle" width="200" height="100"></a>

Description:

Used to mark the start of a flow. It should be noted that only one start node should be in a certain flow.


### End Node: 

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/endn.png" align="middle" width="200" height="100"></a>

Description:

Used to mark the end of a flow. It should be noted that only one start node should be in a certain flow.


### Output Image Node: 

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/outputimagen.png" align="middle" width="200" height="100"></a>

Description:

Used to display an image when the previous node that its connected to has an output data in a form of an image.


### Loop Node: 

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/loopn.png" align="middle" width="200" height="100"></a>

Description:

Used to re-execute the part of the flow (nodes) that lies after it indefinetly. To stop the loop, the stop button on the main GUI should be clicked on.

### Camera Video Input Node: 

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/cameravideoinputn.png" align="middle" width="200" height="100"></a>

Description:

Used for real time camera input in the form of a stream/video. When present in a flow, the input of model for prediction would be the frames from a camera video stream.

Parameters:

Camera index: To specify the index of a connected camera to the computer.


### Select Camera Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/cameraselectn.png" align="middle" width="200" height="100"></a>

Description:

Used for selecting a camera used to take a photo by to be used as an input for nodes such as those for prediction.

Parameters:

Camera index: To specify the index of a connected camera to the computer.





## Computer Vision Library

### Input Model Node: 

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/inputmodeln.png" align="middle" width="200" height="100"></a>

Description:

Used to select a model file to be used for prediction.

Parameters:

Model path: To specify the path for the model file by selecting it in the file explorer window.


### Torch Classify Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/torchclassifyn.png" align="middle" width="200" height="200"></a>

Description:

Used for prediction using Torch classification models. Classifies images into the classes that the model is trained on.

Parameters:

Image path: To specify the path for the image file to be predicted on by selecting it in the file explorer window. Dont select anything to use a photo taken by a camera.

Device: To specify either to use the cpu or cuda for predictions. Select cuda for Nvidia gpu processing if you have a gpu for faster results; otherwise, select cpu.



### Select Model Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/selectmodeln.png" align="middle" width="200" height="300"></a>

Description:

Used to select a pretrained Torch model for training or predicting.

Parameters:

Task: To select the desired computer vision task.

Model: To select the pretrained model for the selected computer vision task.

Builder: To select a specific builder for the pretrained model selected.



### Train Torch Classify Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/traintorchclassifyn.png" align="middle" width="200" height="300"></a>

Description:

Used to train models for classification task by using transfer learning using pretrained torch models.

Parameters:

Dataset Path: To specify the path for the dataset folder by selecting it in the file explorer window. Dont select anything if you have a ClassificationPrepareTorch node in the flow.

Epochs number: To select the number of epochs to train the model for.

Device: To specify either to use the cpu or cuda for training. Select cuda for Nvidia gpu processing if you have a gpu for faster results; otherwise, select cpu.



### Torch Detect Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/torchdetectn.png" align="middle" width="200" height="200"></a>

Description:

Used for prediction using Torch object detection models. Detects objects in images.

Parameters:

Image path: To specify the path for the image file to be predicted on by selecting it in the file explorer window. Dont select anything to use a photo taken by a camera.

Device: To specify either to use the cpu or cuda for predictions. Select cuda for Nvidia gpu processing if you have a gpu for faster results; otherwise, select cpu.



### Train Torch Detect Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/traintorchdetectn.png" align="middle" width="200" height="300"></a>

Description:

Used to train models for object detection task by using transfer learning using pretrained torch models.

Parameters:

Dataset Path: To specify the path for the dataset folder by selecting it in the file explorer window.

Epochs number: To select the number of epochs to train the model for.

Device: To specify either to use the cpu or cuda for training. Select cuda for Nvidia gpu processing if you have a gpu for faster results; otherwise, select cpu.



### Train YOLO Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/trainyolon.png" align="middle" width="400" height="700"></a>

Description:

Used to train models for classification, detection, and segmentation tasks by using transfer learning using pretrained YOLOV8 models.

Parameters:

Mode: To select the desired computer vision task.

Model: To select the pretrained model after selecting a task.

Dataset path: To specify the path for the dataset folder/file by selecting it in the file explorer window. Dont select anything if you have a YOLO node from the Dataset Library in the flow.

Epochs: To select the number of epochs to train the model for.

Image size: To select the size of input images during training.

Batch size: To select the number of images per batch during training.

Device: To specify either to use the cpu or cuda for training. Select cuda for Nvidia gpu processing if you have a gpu for faster results; otherwise, select cpu.



### Predict YOLO Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/predictyolon.png" align="middle" width="250" height="400"></a>

Description: 

Used to perform predictions using pretrained or costum trained YOLOV8 based models for classification, detection, or segmentation.

Parameters:

Model: To select whether to use a pretrained or custom model.

Mode: To select the desired computer vision task.

Select Model: To select the pretrained model in case of predictions using a pretrained model.  

Image path: To specify the path for the image file to be predicted on by selecting it in the file explorer window. Dont select anything to use a photo taken by a camera.



### Segment Anything Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/segmentanythingn.png" align="middle" width="200" height="100"></a>

Description:

Used to segment an image by using the Segment Anything Model (SAM).

Parameters:

Image path: To specify the path for the image file to be predicted on by selecting it in the file explorer window. Dont select anything to use a photo taken by a camera.





## Communication Library

### MQTT Publish Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqttpublishn.png" align="middle" width="300" height="700"></a>

Description: 

Used to publish (send) messages on a topic to an MQTT broker.

Parameters:

Client ID: To specify a client ID. A random ID will be assigned if left empty.

Username: To set a username for broker authentication (optional). Leave empty if not desired.

Password: To set a password for broker authentication (optional). Leave empty if not desired.

Broker: To specify the hostname or IP address of the broker.

Port: To specify the network port of the server host to connect to.

Message: To specify the message to be sent. Input the name of a variable to send as a message or a string.

Topic: To specify the topic to publish on.



### MQTT  Subscribe Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqttsubscriben.png" align="middle" width="300" height="600"></a>

Description:

Used to subscribe to a topic to recieve messages published to those topics.

Parameters:

Client ID: To specify a client ID. A random ID will be assigned if left empty.

Username: To set a username for broker authentication (optional). Leave empty if not desired.

Password: To set a password for broker authentication (optional). Leave empty if not desired.

Broker: To specify the hostname or IP address of the broker.

Port: To specify the network port of the server host to connect to.

Topic: To specify the topic to subscribe to.





## Dataset Library

### ClassificationPrepareYOLO Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/classificationprepareyolon.png" align="middle" width="300" height="500"></a>

Description:

Used to prepare datasets to use for training classification models by using pretrained YOLOV8 classification models. The node will structure the dataset folder to be used with the Train YOLO 
Node.

Parameters:

Dataset path: To specify the path for the dataset folder by selecting it in the file explorer window.

Dataset name: To specify the name of the folder to save the dataset as.

Dataset folder structure: To select whether the images that make up the dataset are organized as a pool of labeled images or in class folders.

Train images percentage: To specify the percentage of the training images from the total images of the dataset.

Test images percentage: To specify the percentage of the test images from the total images of the dataset.



### ClassificationPrepareTorch Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/classificationpreparetorchn.png" align="middle" width="300" height="500"></a>

Description:

Used to prepare datasets to use for training classification models by using pretrained Torch classification models. The node will structure the dataset folder to be used with the Train Torch 
Classify Node.

Parameters:

Dataset path: To specify the path for the dataset folder by selecting it in the file explorer window.

Dataset name: To specify the name of the folder to save the dataset as.

Dataset folder structure: To select whether the images that make up the dataset are organized as a pool of labeled images or in class folders.

Train images percentage: To specify the percentage of the training images from the total images of the dataset.

Test images percentage: To specify the percentage of the test images from the total images of the dataset.



### YOLO From Label Studio Node:

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/yolofromlabelstudion.png" align="middle" width="200" height="300"></a>

Description:

Used to prepare datasets to use for training object detection models by using pretrained YOLOV8 object detection models. The node will create a config.yaml file to use as the dataset input.

Parameters:

Dataset folder: To specify the path for the dataset folder by selecting it in the file explorer window.

Train images percentage: To specify the percentage of the training images from the total images of the dataset.

Test images percentage: To specify the percentage of the test images from the total images of the dataset.


 




