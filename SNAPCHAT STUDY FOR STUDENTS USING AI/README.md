# AI-based-SNAP-STUDY-APP-FOR-STUDENTS

**PROJECT DESCRIPTION**

Main aim and Objective of the Project is to create student community platforms that students could be used in connecting in sharing ideas and knowledge for learning and examination purposes. It has not been easy for the student to improve their knowledge cap in terms of education technologies. As students aim to tackle some problems that our project thoughts and there by provide novel solutions for students .The course material that is presented to students worldwide, specially to students in higher classes or colleges, is often non indulging and monotonous. It has hardly any interactability and often does not drive the student towards further reading on the topics.

Our A.I based app use proprietary Deep Learning models that allows users to create flashcards & summaries by simply taking images of their notes/lecture slides.The app encourages knowledge-based learning,which results in greater understanding & retention of content.The also app has a gamification element that motivates & makes revision fun for users, & gives each user personalized revision content


**Solution and Technology Stack Used:**


1)Authentication Using Firebase, the user is securely authenticated via Oauth options such as Google & Twitter, as well as continue as a Guest. Authentication process is done in Google Cloud Functions.

2)OCR A user chooses images of their notes/lecture slides(handwritten or printed), and their images are converted into text using a Cloud Run container that uses the Google Cloud Vision API.

3)Generation The text is sent to two Docker Images on Cloud Run that run proprietary Deep Learning models to generate What style and gap-filled queries to be used with flashcards, or a summary of the text.


To filter out the background during the live stream of educational videos


Given the parameters and constraints presented by the problem, in terms of quality of the output, speed (in terms of fps) of the output, and cost of the resources required (CPU/GPU cost) , we chose to implement a version DeepLabV3 which is based on the encoder decoder architecture. The video if fed to the model frame by frame and the primary person (educator) is identified and segmented. The background is subtracted in this way from every frame and the output frames are compressed together to form the video which would not have any background objects or people. Implementing DeepLabV3 also ensures that the latency caused by this processing is reduced to a fraction of a second. 


**Instructions to run:**
1. Run `sudo pip3 install -r requirements.txt` to install all packages.
2. Run  `python inference_video.py` for video files.
3. Run `python inference_webcam.py` for live streaming.



**Futuristic and Upscaling Design features Explained Using Model Architecture**
![alt text](https://www.oreilly.com/library/view/hands-on-image-processing/9781789343731/assets/d929fc98-db73-4c77-9d60-4b4582fa03e2.png)

