# Segnet
Classification of lung area only in lung CT

## Title
1. Abstract
2. Project content and method
3. Results and Discussion
4. Conclusion
5. References





## 1. Abstract
  (Eng)This project started as a basic project for segmentation of Putamen tissue in MSA patients. The image segmentation algorithm is based on autoencoder. Autoencoder is an unsupervised learning ai algorithm, and takes the form of transforming the dimension of input data and then restoring it back to its original state. By applying this, segnet allows the user to obtain the desired data by restoring only a specific part of the image, not the original image. As the train data used in the project, 240 256 × 256 lung CT images and 27 were used for validation [1], and an accuracy of about 0.98 was obtained through learning of 100 epochs.
  
(Ko)본 프로젝트는 MSA환자의 피각 조직 분할 연습을 위해 수행하였다. 이미지 분할 알고리즘은 Autoencoder를 기반으로 한다. Autoencoder는 비지도학습 인공지능 알고리즘으로 입력 데이터의 차원을 변환한 다음 원래 상태로 복원하는 형태를 취한다. Segnet을 사용함으로써 사용자는 이미지에서 특정 인스턴스를 추출할 수 있다. 본 프로젝트에 사용된 학습 데이터는 240개의 256x256 폐 CT 이미지와 테스트를 위해 27개의 같은 shape의 폐CT 데이터를 사용하였으며[1], 100 epoch 학습을 통해 약 0.98의 정확도를 얻을 수 있었다.

## 2. Introduction
### 1) Content

