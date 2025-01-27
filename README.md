# Live Face Recogniton

## Inspiration
* [OpenFace](https://github.com/cmusatyalab/openface)
* I refer to the facenet repository of [davidsandberg](https://github.com/davidsandberg/facenet).
* also, [shanren7](https://github.com/shanren7/real_time_face_recognition) repository was a great help in implementing.
## Dependencies
* Tensorflow 1.2.1 - gpu
* Python 3.5
* Same as [requirement.txt](https://github.com/davidsandberg/facenet/blob/master/requirements.txt) in [davidsandberg](https://github.com/davidsandberg/facenet) repository.

## Pre-trained models
* Inception_ResNet_v1 CASIA-WebFace-> [20180402-114759](https://drive.google.com/open?id=1vXMsKEOcqyRBVEwwiBO8Mbyb8YFWuVIK)

## Face alignment using MTCNN
* You need [det1.npy, det2.npy, and det3.npy](https://github.com/davidsandberg/facenet/tree/master/src/align) in the [davidsandberg](https://github.com/davidsandberg/facenet) repository.
## How to use


* First, we need align face data. So, if you run 'Make_aligndata.py' first, the face data that is aligned in the 'output_dir' folder will be saved.
* Second, we need to create our own classifier with the face data we created. <br/>(In the case of me, I had a high recognition rate when I made 30 pictures for each person.)
</br>Your own classifier is a ~.pkl file that loads the previously mentioned pre-trained model ('[20180402-114759](https://drive.google.com/open?id=1vXMsKEOcqyRBVEwwiBO8Mbyb8YFWuVIK)') and embeds the face for each person.<br/>All of these can be obtained by running 'Make_classifier.py'.<br/>
* Finally, we load our own 'my_classifier.pkl' obtained above and then open the sensor and start recognition.
</br> (Note that, look carefully at the paths of files and folders in all .py)
## Result Video Link (Running Man Face Recognition Video)
https://www.youtube.com/watch?v=bei4PLm1OiE&feature=youtu.be

![runningman1.png](description/runningman1.png)
![runningman2.png](description/runningman2.png)

# Arduino Door Lock
![arduino1.png](description/arduino1.png)
![arduino2.png](description/arduino2.png)
https://www.amazon.com/ARCELI-ESP8266-Development-Compatible-Arduino/dp/B07J2QKNHB

## Result Video Link (Face Recognition Door Lock Video)
https://youtu.be/JDSLfVQpbV0
![door_screenshot.png](door_screenshot.png)
