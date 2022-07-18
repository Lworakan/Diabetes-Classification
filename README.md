# Diabetes-Classification
It_camp 16/07/22
Logistic Regression Model
- Classification โดย output จริงๆแล้วออกมาเป็น Regression (จำนวนตัวเลข) จากนั้นนำไป mapping กับ Sigmoid function (หลักคณิตศาสตร์) ก็จะได้ว่าข้อมูลอันนี้เป็นคลาสนี้ หรือ ไม่ได้เป็นคลาสนี้นั้นเอง (เป็นไปได้แค่ 2 คลาสเท่านั้น)
![image](https://user-images.githubusercontent.com/78127819/179487301-559af457-fcb3-4068-897b-aa8460130c95.png)
![image](https://user-images.githubusercontent.com/78127819/179487327-07f4c873-5ead-4510-a914-9804f627017c.png)

Decision Tree Model
- Decision Tree คือ การค่อยๆ แบ่งข้อมูลออกทีละ 2 ส่วน (recursive binary split) จาก node ล่างสุดของ tree เรียกว่า root node และไล่ขึ้นมาเรื่อยๆ จนถึง leaf node ตามภาพ 1 ด้านซ้าย และทำ prediction ค่า target variable ด้วยวิธีการง่ายๆ คือ ใช้ค่า mean ของ target variable node… โดยการ split ข้อมูลจาก root node จนถึง leaf node จะทำจนกว่าจะได้ condition ที่กำหนด เช่น ความลึกของ tree ไม่เกิน 10 ชั้น (max dept) หรือ จำนวนข้อมูลในแต่ละกลุ่มที่แบ่งออกมา (leaf node) มีจำนวนขั้นต่ำ 5 observation (min sample)

K-Nearest Neighbor (K-NN) Model
- K-Nearest Neighbors (K-NN) เป็นวิธีการแบ่งคลาสสำหรับใช้จัดหมวดหมู่ข้อมูล (Classification)ใช้หลักการเปรียบเทียบข้อมูลที่สนใจกับข้อมูลอื่นว่ามีความคล้ายคลึงมากน้อยเพียงใด หากข้อมูลที่กำลังสนใจนั้นอยู่ใกล้ข้อมูลใดมากที่สุด ระบบจะให้คำตอบเป็นเหมือนคำตอบของข้อมูลที่อยู่ใกล้ที่สุดนั้นลักษณะการทำงานแบบไม่ได้ใช้ข้อมูลชุดเรียนรู้ (training data) ในการสร้างแบบจำลองแต่จะใช้ข้อมูลนี้มาเป็นตัวแบบจำลองเลย
![image](https://user-images.githubusercontent.com/78127819/179487772-1f44e46d-d5e5-42dc-a53a-620104d134d8.png)

Reference
https://kongruksiam.medium.com/%E0%B8%AA%E0%B8%A3%E0%B8%B8%E0%B8%9B-machine-learning-ep-4-%E0%B9%80%E0%B8%9E%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%99%E0%B8%9A%E0%B9%89%E0%B8%B2%E0%B8%99%E0%B9%83%E0%B8%81%E0%B8%A5%E0%B9%89%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B8%AA%E0%B8%B8%E0%B8%94-k-nearest-neighbors-787665f7c09d
https://medium.com/@witchapongdaroontham/%E0%B8%A3%E0%B8%B9%E0%B9%89%E0%B8%88%E0%B8%B1%E0%B8%81-decision-tree-random-forrest-%E0%B9%81%E0%B8%A5%E0%B8%B0-xgboost-part-1-cb49c4ac1315
https://medium.com/mmp-li/logistic-regression-%E0%B9%84%E0%B8%A1%E0%B9%88%E0%B8%A1%E0%B8%B5%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3%E0%B9%80%E0%B8%9B%E0%B9%87%E0%B8%99%E0%B9%84%E0%B8%9B%E0%B8%95%E0%B8%B2%E0%B8%A1%E0%B8%AD%E0%B8%A2%E0%B9%88%E0%B8%B2%E0%B8%87%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B8%84%E0%B8%B4%E0%B8%94%E0%B9%80%E0%B8%AA%E0%B8%A1%E0%B8%AD-machine-learning-101-bba2f666234d
