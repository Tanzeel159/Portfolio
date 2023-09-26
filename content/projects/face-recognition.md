---
title: "Face Recognition Based Attendance System"
description: "Using face recognition to mark attendance"
dateString: Jan 2019
draft: false
tags: ["Python", "Anaconda", "Microsoft Face API", "Azure Cloud", "Openpyxl", "Sqlite3", "OpenCV","Microsoft Excel"]
showToc: false
weight: 201
cover:
    image: "/projects/face-recognition/faces.png"
--- 
🔗 [GitHub](https://github.com/Tanzeel159/Face-Recognition-Based-Attendance-System)

## Description

Attendance is primarily important for both the teacher and student of an educational organization.It is very important to keep record of the attendance. The problem arises when we think about the traditional process of taking attendance in class room which involves calling name/roll number. A face recognition based attendance system could automate the entire system and streamline the process increasing the rate and reducing the time.

Steps followed in marking attendance:

- 20 images are captured for every user to create dataset for training.

![](/projects/face-recognition/add_student.png)
![](/projects/face-recognition/add_faces.png)
![](/projects/face-recognition/dataset.png)

- All the details related to student are captured in database.

- This information is convert to URL which is sent to Azure Cloud where Microsoft Face Detection API is used to train the dataset and extract face features.

![capture](/projects/face-recognition/Capture.png)

- Then when the image is captured, faces are detected, matched against database and attendance is marked.

![Attendance](/projects/face-recognition/attendance.png)