# gun-detection

### Goal
Kids must be safe at school. AI For Mankind wants to build and deploy gun detection system to local schools to protect our children.

### Datasets
1. [YouTube-GDD: A challenging gun detection dataset with rich contextual information](https://github.com/UCAS-GYX/YouTube-GDD).
2. [Hands Guns and Phones (HGP) Dataset](https://drive.google.com/file/d/138Zp7MuchcS4He6LBFSTow5q97BwnpWv).
Prepared by the authors of this paper [TYolov5: A Temporal Yolov5 Detector Based on Quasi-Recurrent Neural Networks for Real-Time Handgun Detection in Video](https://www.researchgate.net/profile/Cuauhtemoc-Suarez-Ramirez-3/publication/356339851_TYolov5_A_Temporal_Yolov5_Detector_Based_on_Quasi-Recurrent_Neural_Networks_for_Real-Time_Handgun_Detection_in_Video).
3. [Real-time gun detection in CCTV : An open problem](https://github.com/Deepknowledge-US/US-Real-time-gun-detection-in-CCTV-An-open-problem-dataset).
4. [Detection-of-lumbar-weapon-pistol-by-deep-learning--With-YOLO-v5](https://github.com/amin-tohidi/Detection-of-pistol-by-deep-learning-With-YOLO_v5).
5. [https://www.kaggle.com/datasets/atulyakumar98/fire-and-gun-dataset/](https://www.kaggle.com/datasets/atulyakumar98/fire-and-gun-dataset/)


### Model
AI For Mankind combined the following datasets into the above one consolidated train dataset and trained an experimental Yolov5 model for gun detection.

1. Hand, gun and phone dataset prepared by
Mario Alberto Duran-Vega, Miguel Gonzalez-Mendoza, Leonardo Chang, Cuauhtemoc Suarez-Ramirez, the authors of TYolov5: A Temporal Yolov5 Detector Based on Quasi-Recurrent Neural Networks for Real-Time Handgun Detection in Video

2. Rifle, gun and fire dataset prepared by Atulya Kumar

Here are the experimental model's metrics. (Yolov5 large, 300 epochs, batch size 8, image size 640)
YOLOv5l_rifle summary: 267 layers, 46119048 parameters, 0 gradients, 107.7 GFLOPs
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 100% 32/32 [00:07<00:00,  4.17it/s]
                   all        500        645      0.834      0.741       0.77      0.496
                   gun        500        195      0.898      0.774      0.837      0.658
                  fire        500        151      0.798      0.722      0.744      0.349
                 rifle        500        299      0.808      0.726       0.73      0.481

Our volunteers are working on a better model. Checkout our Colab notebook in the repo.


### Resources
1. [After Uvalde: Could A.I. prevent another school shooting?](https://fortune.com/2022/05/31/ai-prevent-uvalde-mass-school-shooting/)
2. [Seminole County Public Schools testing AI gun detection system on several campuses](https://www.wesh.com/article/seminole-ai-gun-detection/40120102#)

### Companies offer Gun Detection System.
1. [ZeroEyes](https://zeroeyes.com/)
2. [Omnilert](https://www.omnilert.com/)
3. [Defendry](https://defendry.com/)
4. [Athena Securities](https://www.athena-security.com/)

