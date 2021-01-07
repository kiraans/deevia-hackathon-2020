# Deevia Hackathon 2020 

[![TensorFlow 2.2](https://img.shields.io/badge/TensorFlow-2.2-FF6F00?logo=tensorflow)](https://github.com/tensorflow/tensorflow/releases/tag/v2.2.0)
[![Python 3.6](https://img.shields.io/badge/Python-3.6-3776AB)](https://www.python.org/downloads/release/python-360/)

This is a official repository for the Deevia Hackathon Project.

The problem statement of the hackathon was to develop an android application to detect fire and smoke in real time scenario.

**Our Approach:** We used the Tensorflow Object Detection API to train the existing model (Transfer Learning) i.e., [EfficientDet model](http://download.tensorflow.org/models/object_detection/tf2/20200711/efficientdet_d0_coco17_tpu-32.tar.gz).

As we know that, Object detection is a technique of training computers to detect objects from images or videos; over the years, there are many object detection architectures and algorithms created by multiple companies and researchers. In this race of creating the most accurate and efficient model, the Google Brain team recently released the EfficientDet model, it achieved the highest accuracy with fewest training epochs in object detection tasks. This architecture beats the YOLO, AmoebeaNet with minimum computation power. The architecture for the same is as shown below:
![](https://1.bp.blogspot.com/-MQO5qKuTT8c/XpdE8_IwpsI/AAAAAAAAFtg/mSjhF2ws5FYxwcHN6h9_l5DqYzQlNYJwwCLcBGAsYHQ/s1600/image1.png)

It is an advanced version of EfficientNet, which was the state of art object detection model in early 2019, EfficientNet was a baseline network created by Automl MNAS, it achieved state-of-the-art 84.4% more accuracy and used a highly effective compound coefficient to scale up CNNs in a more structured manner.
The comparision of different state-of-the-art models is as shown in the image below:
![https://blog.roboflow.com/training-efficientdet-object-detection-model-with-a-custom-dataset/](https://github.com/kiraans/deevia-hackathon-2020/blob/main/model/efficientdet-performance.png)

**Regarding the Data-set:** We re-annotated the existing [Fire dataset](https://github.com/OlafenwaMoses/FireNET/releases/download/v1.0/fire-dataset.zip) to Fire and Smoke dataset using [LabelImg](https://github.com/tzutalin/labelImg). We used 320 samples for training and 30 samples for validation. 
We achieved a loss of ***0.14*** after training for approximately 5000 steps. The training was done on Google Colaboratory.

**Steps to Run the code:**
1. Clone the github repository.
2. Download the weights and move them to training folder and edit the path in .config file.
3. Run the ipynb file either in local system or Colab. Install the dependencies as stated in the notebook.
4. For testing the model, run the Testing portion of the notebook.

**Results:**
Following are a few results from the model.

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(1).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(3).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(15).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(6).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(28).png "Results")
