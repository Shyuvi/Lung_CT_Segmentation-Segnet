# Segnet
Classification of lung area only in lung CT

## Title
1. Abstract
2. Content
3. Result
4. References



## 1. Abstract
  (Eng)This project started as a basic project for segmentation of Putamen tissue in MSA patients. The image segmentation algorithm is based on autoencoder. Autoencoder is an unsupervised learning ai algorithm, and takes the form of transforming the dimension of input data and then restoring it back to its original state. By applying this, segnet allows the user to obtain the desired data by restoring only a specific part of the image, not the original image. As the train data used in the project, 240 256 × 256 lung CT images and 27 were used for validation [1], and an accuracy of about 0.98 was obtained through learning of 100 epochs.
  
(Ko)본 프로젝트는 MSA환자의 피각 조직 분할 연습을 위해 수행하였다. 이미지 분할 알고리즘은 Autoencoder를 기반으로 한다. Autoencoder는 비지도학습 인공지능 알고리즘으로 입력 데이터의 차원을 변환한 다음 원래 상태로 복원하는 형태를 취한다. Segnet을 사용함으로써 사용자는 이미지에서 특정 인스턴스를 추출할 수 있다. 본 프로젝트에 사용된 학습 데이터는 240개의 256x256 폐 CT 이미지와 테스트를 위해 27개의 같은 shape의 폐CT 데이터를 사용하였으며[1], 100 epoch 학습을 통해 약 0.98의 정확도를 얻을 수 있었다.

## 2. Content
  (Eng)Segnet aims to segment objects in an image into meaningful units. In other words, it predicts which class each pixel in the image belongs to. Since the purpose of this project is to segment only the lung position on the CT image, in the output image, the value of the pixel to which the lung belongs is 1, and all other pixel values are 0.
  The structure of Segnet is divided into Encoding Part and Decoding Part as shown in Figure 1. Each part is responsible for compressing the original image and restoring the compressed image.
  
  (Ko)Segnet은 이미지 내의 물체들을 의미 있는 단위로 분할해 내는 것을 목적으로 한다. 즉, 이미지의 각 픽셀이 어느 클레스에 속하는지 예측하는 것이다. 본 프로젝트에서는 CT 이미지상에서 폐의 위치만 분할하는 것이 목적이기에 출력 이미지는 폐가 속한 픽셀의 값은 1, 그 이외의 픽셀값은 전부 0으로 나타내어 진다.
 Segnet의 구조는 그림 1과 같이 Encoding 파트와 Decoding 파트 2개로 나뉜다. 각각의 파트는 원본 이미지를 압축시키고 압축된 이미지를 복원하는 역할을 담당한다. 
 

 
 ![image](https://user-images.githubusercontent.com/58457155/180983945-5bcd6834-48d4-4d31-8f71-56e6427f3abf.png)Fig 1. Segnet Architecture[2]
 
  ## 3. Result
   (Eng)As shown in Fig 2, DSC of about 0.98 can be confirmed, and the validation result is also shown with a similar value. The overall learning proceeded smoothly and there was no overfitting.
   
   (Ko)그림 2와 같이 약 0.98의 DSC를 확인할 수 있고 validation 결과 역시 비슷한 수치로 나타나고 있다. 전체적인 학습이 원활하게 진행되었고 overfitting 또한 되지 않았다.
 
 ![image](https://user-images.githubusercontent.com/58457155/181034867-bbc5b9c9-7025-43d7-816b-c84a5203c9fa.png)
 Fig 2. Training result  figure
 ![image](https://user-images.githubusercontent.com/58457155/181035496-a1a69884-8096-4eb6-97e1-05da535b0904.png)
Fig 3. Predict results

## 4. References
[1] https://github.com/kairess/CT_lung_segmentation/tree/master/dataset
[2] V. Badrinarayanan, A. Kendall and R. Cipolla, "SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation," in IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 39, no. 12, pp. 2481-2495, 1 Dec. 2017, doi: 10.1109/TPAMI.2016.2644615.
