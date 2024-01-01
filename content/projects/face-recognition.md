---
title: "Face Recognition Based Attendance System"
description: "Using face recognition to mark attendance"
dateString: Jan 2019
draft: false
tags: ["Python", "Anaconda", "Microsoft Face API", "Azure Cloud", "Openpyxl", "Sqlite3", "OpenCV","Microsoft Excel"]
showToc: false
weight: 404
cover:
    image: "/projects/face-recognition/faces.png"
--- 
🔗 [GitHub](https://github.com/Tanzeel159/Face-Recognition-Based-Attendance-System)

### Description

Attendance is primarily important for both the teacher and student of an educational organization. It is very important to keep record of the attendance. The problem arises when we think about the traditional process of taking attendance in class room which involves calling name/roll number. A face recognition based attendance system could automate the entire system and streamline the process increasing the rate and reducing the time.

### Team Members

- Tanzeel Ahmed Shaikh (code developent and testing)
- Kyatham Priyanka (dataset collection)
- Ramakrishna (code development)
- Manikanta (documentation) 

### Algorithm

Azure Face API is used to detect, recognize and analyze human faces in images.

1) Get Face Attributes
2) Authorize the Face API Call
3) Create the Person Group
4) Define people for Person Group
5) Detect faces and register them to correct person
6) Train the Person Group
7) Identify face against defined group

### Module Design

Student Registration Flow

![Alt text](/projects/face-recognition/image-1.png)

Faculty Attendance Capture Flow

![Alt text](/projects/face-recognition/image-2.png)

Feature Extraction

![Alt text](/projects/face-recognition/image-3.png)

Generating Attendance

![Alt text](/projects/face-recognition/image-4.png)


### Process

- 20 images are captured for every user to create dataset for training.

![](/projects/face-recognition/add_student.png)
![](/projects/face-recognition/add_faces.png)
![](/projects/face-recognition/dataset.png)

- All the details related to student are captured in database.

- This information is converted to URL which is sent to Azure Cloud where Microsoft Face Detection API is used to train the dataset and extract face features.

![capture](/projects/face-recognition/Capture.png)

- When the image is captured, faces are detected, matched against database and attendance is marked.

### Results

![Attendance](/projects/face-recognition/attendance.png)

