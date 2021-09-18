# Face-emotion-yolov5
In this project, I used the Yolov5 object detection algorithm to detect a person's feelings through a face if he is happy, normal, or sad. 

# The steps of this project      
First, I started collecting datasets from google, focused on three categories happy, sad, and normal and each category collected about 200 images.  
Second, I uploaded the dataset to the Labelbox and then put a boundary box on all the image  
Third: - I have exported the Jason file that contains the boundary box information then I uploaded it to roboflow so that I can convert the Jason file  to Yolov5 annotation format   
Fourth: - I used this colab  https://colab.research.google.com/drive/1gDZ2xcTOgR39tGGs-EZ6i3RTs16wmzZQ to help me to train YOLOv5 on Custom Objects 

fifth: - after I finished my train I saved my model and created a new  notebook to use my model by upload image or video or use Webcam  
this the result of one of the image that model predicted right

<img width="457" alt="Screen Shot 2021-09-18 at 10 55 55 PM" src="https://user-images.githubusercontent.com/70725011/133907066-f03f9957-1216-49c7-983a-eab06f883737.png">

# Run the model 
to run my model there two ways
 First way  Download the yolov5 repository and make sure to install all libraries then run the command  
python3 detect.py --source 1 --weights /* bath for the weight /yolov5/best.pt
this will open the webcam for you 

if you want to use photo or video you can check the yolov5 repository tutorial  

Second way  you can run  yolov5_face_emotion.ipynb notebook but you need change the path for the weight

# Note 
this project is not worked perfectly for all face emotions because i trained  the model for 500 photo for all categories and this not enough it need more than 1500 photos for each category to work perfectly. The purpose for this project to understand how the yolov5 works and how can apply the model use photos and videos and webcam.
