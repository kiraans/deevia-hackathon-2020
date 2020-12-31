# Deevia Hackathon 2020 

[![TensorFlow 2.2](https://img.shields.io/badge/TensorFlow-2.2-FF6F00?logo=tensorflow)](https://github.com/tensorflow/tensorflow/releases/tag/v2.2.0)
[![Python 3.6](https://img.shields.io/badge/Python-3.6-3776AB)](https://www.python.org/downloads/release/python-360/)
[![Google Colaboratory](https://colab.research.google.com/assets/colab-badge.svg)]

This is a official repository for the Deevia Hackathon Project.

The problem statement of the hackathon was to develop an android application to detect fire and smoke in real time scenario.

**Our Approach:** We used the Tensorflow Object Detection API to train the existing model (Transfer Learning) i.e., [EfficientDet model](http://download.tensorflow.org/models/object_detection/tf2/20200711/efficientdet_d0_coco17_tpu-32.tar.gz).
We re-annotated the existing [Fire dataset](https://github.com/OlafenwaMoses/FireNET/releases/download/v1.0/fire-dataset.zip) to Fire and Smoke dataset using [LabelImg](https://github.com/tzutalin/labelImg). We used 320 samples for training and 30 samples for validation. 
We achieved a loss of ***0.14*** after training for approximately 5000 steps.

**Results:**
Following are a few results from the model.

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(1).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(3).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(15).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(6).png "Results")

![alt text](https://github.com/kiraans/deevia-hackathon-2020/blob/main/result-images/download%20(28).png "Results")
