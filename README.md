# Traffic_sign_detection_CNN_GUI


You must have heard about the self-driving cars in which the passenger can fully depend on the car for traveling. But to achieve that level of autonomous driving, it is necessary for vehicles to understand and follow all traffic rules.
In the world of Artificial Intelligence and advancement in technologies, many researchers and big companies like Tesla, Uber, Google, Mercedes-Benz, Toyota, Ford, Audi, etc are working on autonomous vehicles and self-driving cars. So, for achieving accuracy in this technology, the vehicles should be able to interpret traffic signs and make decisions accordingly.

**What is Traffic Signs Recognition?**
There are several different types of traffic signs like speed limits, no entry, traffic signals, turn left or right, children crossing, no passing of heavy vehicles, etc. Traffic signs classification is the process of identifying which class a traffic sign belongs to.

**Traffic Signs Recognition – About the Project**
In this Python project example, we will build a deep neural network model that can classify traffic signs present in the image into different categories. With this model, we can read and understand traffic signs which are a very important task for all autonomous vehicles.


**TRAFFIC SIGN CLASSIFIER GUI**

Now we are going to build a graphical user interface for our traffic signs classifier with Tkinter. Tkinter is a GUI toolkit in the standard python library. Make a new file in the project folder and copy the below code. Save it as gui.py and you can run the code by typing python gui.py in the command line.
In this file, we have first loaded the trained model ‘traffic_classifier.h5’ using Keras. And then we build the GUI for uploading the image and a button is used to classify which calls the classify() function. The classify() function is converting the image into the dimension of shape (1, 30, 30, 3). This is because to predict the traffic sign, we must provide the same dimension we have used when building the model. Then we predict the class, the model.predict_classes(image) returns us a number between (0-42) which represents the class it belongs to. We use the dictionary to get the information about the class. Here’s the code for the gui.py file.

![image](https://user-images.githubusercontent.com/87114918/146131914-83271d05-6a1a-4fe7-aa71-f69ac166c079.png)

**SUMMARY**

In this Project, we have successfully classified the traffic signs classifier with 95% accuracy and visualized how our accuracy and loss changes with time, which is pretty good from a simple CNN model.

