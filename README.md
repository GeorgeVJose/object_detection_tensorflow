# Object Detection Tensorflow with video inputs.
This is an Object Detection program taken from Tensorflow GitHub. It takes frames from a video, run object detection and write back the frame into the time sequence.

## Getting Started
This repository contains program to read frames from a video and write back to the time sequence.
> **Note :**
> - The master directory which contains all the other programs along with the tensorflow graph should be downloaded from [here](https://github.com/tensorflow/models/tree/master/object_detection).

~~~ sh
$ git clone https://github.com/tensorflow/models/tree/master/object_detection ./object_detection
$ git clone https://github.com/georgevjose/object_detection_tensorflow/object_new.py ./object_detection/
~~~

## Packages
Eventhough opencv is the best package for the job, opencv spits out errors in Ubuntu in Windows (WSL). So, an alternate solution is [ImageIO](https://pypi.python.org/pypi/imageio).
~~~ sh
$ pip install imageio
~~~

Aditionally basic libraries like Tensorflow, numpy are required.
~~~ sh
$ pip install tensorflow, numpy, matplotlib, PIL
$ apt-get install python-opencv
~~~

# Execution
Edit the python code at object_detection/object_new.py and add the path to the video file and path to write video file. If the tensorflow model graph is not found, it will automatically download the graph from [here](http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v1_coco_11_06_2017.tar.gz) [Size : 122MB].
Now just run the script.
> **Note : **
> Final Video rendering takes time depending on the length of input video and also your processing capability.

~~~ sh
$ python3 object_new.py
~~~
