# 30.-MIT--Facial-Recognition
#TASKS-

Creating an AI-based facial recognition software involves several steps, follwing are high-level steps to be followed, of the typical process:

Define the Objectives: 
1. User should be able to upload the picture and system should be able to find the face from the live and recorded videos with time stamp.
2. System should be able to highlight after certiain % match- promt user to confirm the recognition- model should self learn based on the user selection.
![image](https://github.com/Novius-ISSS-AI/30.-MIT--Facial-Recognition/assets/129680262/76b0e3b7-8f01-4fa4-8d80-62892bb2b026)

Data Collection: Gather a large and diverse dataset of facial images to train your model. Include a wide range of variations in lighting conditions, angles, expressions, ethnicities, and ages to ensure robustness and accuracy.

Data Preprocessing: Clean and preprocess the collected data. This may involve cropping and aligning the faces, normalizing image size and color, and removing noise or irrelevant information.

Annotation: Annotate the dataset by labeling each face with the appropriate identity or characteristics you want the software to recognize (e.g., gender, age, emotions). This is a time-consuming task but is essential for training a supervised learning model.

Model Selection: Choose an appropriate machine learning model for facial recognition. Popular choices include convolutional neural networks (CNNs), particularly deep learning architectures like VGGNet, ResNet, or Inception. Consider factors such as model accuracy, computational requirements, and available resources.

Model Training: Train your selected model using the annotated dataset. This involves feeding the labeled images into the model, adjusting the model's weights through backpropagation, and optimizing the model's performance using techniques like gradient descent. This step may require substantial computational power and time.

Model Evaluation: Assess the trained model's performance by evaluating its accuracy, precision, recall, and other relevant metrics. Use a separate validation dataset to measure the model's generalization ability and identify any overfitting or underfitting issues.

Hyperparameter Tuning: Adjust the hyperparameters of the model, such as learning rate, batch size, and network architecture, to optimize performance. This process often involves trial and error, experimenting with different configurations to find the best combination.

Testing and Validation: Test the final trained model on an independent test dataset that was not used during training or validation. Evaluate the model's accuracy, robustness, and computational efficiency.

Deployment: Integrate the trained model into a software application or system. Develop an interface that accepts images or video streams, performs real-time facial recognition, and outputs the results. Ensure that the software handles various scenarios, such as detecting multiple faces, handling occlusions, and maintaining accuracy under different environmental conditions.

Continuous Improvement: Monitor the performance of the deployed system and collect user feedback. Continuously refine and update the model to enhance its accuracy, incorporate new features, and address any limitations or shortcomings.

Remember that developing an AI-based facial recognition software is a complex task that requires expertise in machine learning, computer vision, and software engineering. It's essential to follow ethical considerations, prioritize user privacy and data security, and comply with legal regulations when working with facial recognition technology.

GENERAL INFO-
Facial recognition software (FRS) is defined as a biometric tool used to match faces in images, usually from photos and video stills, against an existing database of identities. It can be broken down into three parts — detection (finding a face in an image), analysis (face mapping), and recognition (confirming identity). 

An example of facial recognition technology is the auto photo tagging feature on Facebook or even Google Photos. 
![image](https://github.com/Novius-ISSS-AI/30.-MIT--Facial-Recognition/assets/129680262/3ccdc3d6-34e9-443b-bcfd-ca88a7ddee90)

How does facial recognition software work?
Any good FRS has three key components:

Hardware to capture the images. These images can also be fed into the software from independent devices.
Intelligence to compare the captured faces with existing data.
Database, i.e., an existing collection of identities. These can be anything from employee databases to images scrubbed from social media. (Please note that scrubbed social media images are unethical.)
![image](https://github.com/Novius-ISSS-AI/30.-MIT--Facial-Recognition/assets/129680262/8d227163-cd82-4c3d-b135-26737d4b7902)


Now, let’s understand how FRS works.

Detection: Detection begins with the extraction of the face out of the image fed into the system. Subsequently, various features on the human face are marked. Certain features of the face do not change with age or size. These include the distance between the eyes, the depth of the eye socket, and the shape of the nose. There are around 80 such features called ‘landmarks.’ The measurements of these landmarks are then put together to create a code. This code is called a ‘faceprint,’ and it is unique to every person.
Matching: This faceprint is then matched with the prints stored in the system. At this stage, the image goes through several layers of technology to ensure accuracy. Since most of our databases are currently 2D photos, the database images need to be processed by a layer of technology. This processing usually involves pulling out the facial landmarks to resemble their 3D counterparts. If the subject image is low resolution, it must be encoded and decoded to produce details with the desired resolution. The algorithms need to consider the differences in lighting, facial expression, and angles.
Identification: The goal of this step depends on what the facial recognition software is used for — surveillance or authentication. This step should ideally produce a 1:1 match for the subject. This may be done in multiple ways, a quick pass to narrow down the options, then enable the more complex layers to take over. Some companies analyze skin texture along with facial recognition algorithms to increase accuracy.
![image](https://github.com/Novius-ISSS-AI/30.-MIT--Facial-Recognition/assets/129680262/86e46d74-7b3e-44b3-a2eb-d675d535222c)

Each facial recognition software provider focuses on different aspects of the technology layers to provide almost-flawless service. For example, one software may focus on correcting lighting conditions while another can focus on skin texture analysis. 
![image](https://github.com/Novius-ISSS-AI/30.-MIT--Facial-Recognition/assets/129680262/975daa84-ce03-406b-8c2c-e6f61c287b47)

REF SOLUTIONS-
Betaface
Amazon Rekognition
Cognitec
BioID
Trueface.ai
Sky Biometry
SenseTime
Kairos
FaceFirst
Face++
DeepVision AI
