# Traffic-control-via-bdd100k
traffic control managment system via bdd 100k dataset 
This project implements a real-time smart traffic management system using YOLOv5 object detection.
It can detect multiple vehicle types from the BDD100K dataset and also recognize ambulances using a custom dataset.
Once detected, it can allocate dynamic green light timing based on traffic density
Detects multiple vehicle types (car, truck, bus, motorcycle, person, etc.)
Works on recorded videos
Displays dynamic green light time above the video feed
Uses PyTorch + OpenCV for real-time performance
Steps to run the project
1.git clone https://github.com/kushalt1011-dev/Smart-Traffic-Signal.git
cd Smart-Traffic-Signal(if direcltly)
2.install dependencies pip install -r requirements.txt
3.Download BDD100K dataset
You can download the dataset from Kaggle or from the official BDD100K site.
4.Update dataset.yaml
Create a dataset.yaml file in the project root:
5.Training the Model
6.download yolov5 and  train the YOLOv5 model with your combined dataset.
7.On a YouTube live stream
//We use cap_utils.py for YouTube capture:
Live Traffic Management
traffic.py:
Counts vehicles in each lane
Live Traffic Management




Allocates green time dynamically

Prioritizes ambulance lane if detected
