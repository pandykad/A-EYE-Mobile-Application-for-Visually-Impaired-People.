# :eye_speech_bubble: A-EYE-Mobile-Application-for-Visually-Impaired-People.

![Flutter](https://img.shields.io/badge/Software-Flutter-blue?style=flat&logo=Flutter)
![language](https://img.shields.io/badge/language-dart-yellow?style=flat&logo=dart)
![Algorithm](https://img.shields.io/badge/algorithm-OCR-red?style=flat&logo=OCR)

Flutter based mobile application which uses machine learning for object detection provides the name of the object and its position(either left or right side) as an audio output. It also uses optical character recognition to scan text and provides price and expiry date of the product.    

- Flutter framework was used to develop this application, thus, this app will run on Android as well as on iOS platform.  
- TensorFlow Lite and MobileNet provide the necessary dependencies and will do the required object detection.    


#### SYSTEM BLOCK DIAGRAM:  
<img src="images/block_diagram.png" width="400" alt="my image">

### Modules:  
##### :point_right: Module 1:  User Interface  
Android/iOS application is built using Flutter Framework and Google TalkBack utilization. Flutter supports Dart Language.Hence User Interface is created in Dart Language.UI consist of Home Page which cordially invited blind users to start the app. There are two options provided for users:    
1)Start Object Detection !  
2)OCR  
  
##### :point_right: Module 2:  Object Detection  
Given an image or a video stream, an object detection model can identify which of a known set of objects might be present and provide information about their positions within the image.An object detection model is trained to detect the presence and location of multiple classes of objects.When we subsequently provide an image to the model, it will output a list of the objects it detects, the location of a bounding box that contains each object, and a score that indicates the confidence that detection was correct.
For each detected object, the model will return an array of four numbers representing a bounding rectangle that surrounds its position. For the starter model we provide, the numbers are ordered as follows:[top,left,right,bottom]
Object with maximum accuracy is labelled and its speech output is given.
Pretrained model : MobileNet  
  
##### :point_right: Module 3:  OCR  
OCR module is used to convert the text inside the image into an actual text. Our app needs this to recognise the content on the price tags, etc and to extract important information like the product name, contents and price tags. 
To do this we have divided the photo into two halves. The lower half is generally where the price is. This saves extra computations. Further in the lower half, we then focus on the text which is bold or which has a bigger text size than the rest of the text inside the image.  
  
##### :camera: Some sample images of the applications :      
<img src="images/homepage.png" height="300" alt="my image">      <img src="images/object_detection.png" height="300" alt="my image">      <img src="images/ocr.png" height="300" alt="my image">  

## :man_student:  Author
[![Twitter](https://img.shields.io/badge/follow-%40PratikKakade007-1DA1F2?style=flat&logo=Twitter)](https://twitter.com/PratikKakade007) 












