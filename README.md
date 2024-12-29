# AutonomousVehicleDetection

**📚 Project Overview**

This project focuses on detecting and classifying objects in images for autonomous vehicles using deep learning. By leveraging YOLOv5 for real-time object detection, the project aims to enhance the safety and decision-making processes of autonomous vehicles.

**🧰 Tools and Technologies Used**

•	Programming Language: Python

•	Deep Learning Framework: Pytorch

•	Object Detection Model: YOLOv5

•	Libraries: NumPy, Pandas, OpenCV, Matplotlib, Seaborn

•	Deployment/Version Control: Git, GitHub



**📊 Dataset Description**

The dataset includes images and their corresponding label files for object detection. Key classes include:

pickup_truck        : Pickup trucks

car                 :	Cars

articulated_truck	  : Articulated trucks

bus	                : Buses

motorized_vehicle   : Other motorized vehicles

work_van	          : Work vans

single_unit_truck   : Single-unit trucks

pedestrian	        : Pedestrians

bicycle	            : Bicycles

non-motorized_vehicle	:Non-motorized vehicles

motorcycle          :	Motorcycles


Dataset Summary:

•	Total Images: [1000]

•	Total Classes: 11

•	Format: YOLO-compliant (images and labels)



**📈 Project Workflow**


1. Dataset Preparation
   
•	Organized images and labels into train and test directories.

•  dataset/images/train/: For training images.

•  dataset/images/test/: For testing/validation images.

•  dataset/labels/train/: For training annotations (YOLO format).

•  dataset/labels/test/: For testing annotations (YOLO format).

•	Images and labels are converted to YOLO format and saved in respective folders

•	Converted label classes into numeric format as per YOLO requirements.


2. Model Training

•	Trained the YOLOv5 model using the train.py script.

•	Defined training parameters such as:
o	Image size: 640x640
o	Batch size: 16
o	Epochs: 100

•	Utilized custom dataset YAML file for training.Weights after training will be saved in the /train/exp/weights/best.pt file

•	After validation , the predicted images will be saved in the train/exp/

3. Model Evaluation
   
•	Evaluated the model on test data for:
o	Object detection accuracy
o	Mean Average Precision (MAP)

•	Stored results in the runs/detect/exp folder.

4. Testing and Visualization
   
•	Ran inference on test images and visualized detected objects with bounding boxes and confidence scores.

•	After testing the predicted images will be saved in the runs/detect/exp folder


📚 The second part of the project involves analysing the usage of autopilot and its impact on road safety.
The following observations were obtained after performing exploratory data analysin on the data

The number of events occured by date, year, day, country and state.

The distribution and proportion of events.

The frequency of Tesla colliding with other vehicles.

The event distribution across models.

The distribution of verified Tesla autopilot deaths.






