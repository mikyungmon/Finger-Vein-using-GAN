# Finger-Vein-using-GAN
GAN을 이용하여 가짜 지정맥 이미지 생성하기

### ✅ 과정 ###

1. 20명의 실제 지정맥 영상을 frame capture ( 한명당 4개의 영상 )
2. train, validation, test 데이터를 6:2:2 비율로 분할 
3. capture image size를 640 * 480 -> 64 * 64로 resize
4. 모델 훈련
5. 학습된 모델 중 generator(생성자)를 통해 생성된 fake 지정맥 이미지 확인

### ✅ 사용 모델 ###

-  DCGAN(Deep Convolutional Generative Adversarial Network)

    - parameters

       1. epoch : 200 

       2. batch size : 81

       3. learning rate : 0.0001

       4. earlystop patient : 100

       5. generator input dim : 100  ->  생성자에 들어갈 노이즈 벡터 차원수

    - 구조

![image](https://user-images.githubusercontent.com/66320010/136953860-54f6c87b-7597-4a38-9716-c4a457295c3c.png)


