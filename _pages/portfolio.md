---
title: Portfolio
layout: single
author_profile: true
read_time: true
comments: true
share: true
related: true
toc: true
toc_sticky: true
toc_label: Index
last_modified_at: '2020-09-25 00:00:00 +0800'
---

## Instance Segmentation 분야 딥러닝 모델 개발
### Instance Segmentation 모델 학습 데이터 태깅 툴 개발
> [github link](https://github.com/KITECH-AI-LAB/InstanceSegmentationAnnotationTool)

```java
개발 기간
ver 1.0: 2020.03~2020.04
ver 1.1: 2020.08~2020.09
개발 언어: C++(Qt, OpenCV)
입력: 이미지
출력: *.mask: 입력 이미지와 같은 해상도의 mask, *.txt: *.mask에 대한 label, *.dat: mask 생성을 위한 마커(실제 모델 학습에는 필요 없음)
```
![ISAT](../../assets/images/ISAT.png){: .align-center}

---

### 토마토 인식을 위한 딥러닝 기반 Instance Segmentation 모델 학습
> [demo video link](https://youtu.be/ewgW1aQRRyk)

```java
모델 학습
개발 기간: 2020.04~2020.06
개발 언어: Python
인식 대상 토마토: 실제 농장 환경에서 수확 로봇의 워크스페이스에 포함되는 토마토
Class: 숙도 1(USDA 숙도 6단계 중 Green, Breaker), 숙도 2(USDA 숙도 6단계 중 Turing, Pink), 숙도 3(USDA 숙도 6단계 중 Light Red, Red)

모델 변환
개발 기간: 2020.09~2020.09
개발 언어: Python, C++
PyTorch에서 학습한 instance segmentation 모델을 C++ 에서 사용할 수 있도록 변환 및 preprocess, forward, postprocess, visualize 등 함수로 구성된 DLL 작성(ONNX Runtime)
```
![tomato1](../../assets/images/tomato1.jpg){: .align-center}
![tomato2](../../assets/images/tomato2.jpg){: .align-center}

---

### 식판 위 음식물 영역 인식을 위한 딥러닝 기반 Instance Segmentation 모델 학습
<!-- Class: Rice, Soup, Side dish1, Side dish2, Side dish3 -->
```java
개발 기간: 2020.09~현재
개발 언어: Python
Class: Rice
```
![rice1](../../assets/images/rice1.jpg){: .align-center}
![rice2](../../assets/images/rice2.jpg){: .align-center}

---

## Object Detection 분야 딥러닝 모델 개발
### 마스크 검출기
>[article link1](http://naver.me/xBDFbMHS) [article link2](http://naver.me/xN9fk3cb)

```java
개발 기간: 2020.08~2020.08
개발 언어: C++
Class: 마스크(양품), 마스크(불량품)
```
![mask1](../../assets/images/mask1.png){: .align-center}
![mask2](../../assets/images/mask2.png){: .align-center}

---

### 수중 기둥 검출기
```java
개발 기간: 2020.09~2020.09
개발 언어: C++
Class: 수중 기둥
```
![underwater_pillar1](../../assets/images/underwater_pillar1.jpg){: .align-center}
![underwater_pillar2](../../assets/images/underwater_pillar2.jpg){: .align-center}

---

### 일반 객체 검출기
```java
개발 기간: 2019.08~2019.10
개발 언어: C++, Python
Class: 사람, 차량, 트럭, 버스, 휠체어, 유모차, 불꽃
```
![object1](../../assets/images/object1.jpg){: .align-center}
![object2](../../assets/images/object2.jpg){: .align-center}

---

### 얼굴 검출기
```java
개발 기간: 2019.04~2019.06
개발 언어: C++
Class: 얼굴
```
![face1](../../assets/images/face1.jpg){: .align-center}
![face2](../../assets/images/face2.jpg){: .align-center}

---

### 사람 검출기
```java
개발 기간: 2019.01~2019.02
개발 언어: C++
Class: 아이(미취학아동), 어른(아이에 해당하지 않는 사람)
```
![person1](../../assets/images/person1.jpg){: .align-center}
![person2](../../assets/images/person2.jpg){: .align-center}

---

## Classification 분야 딥러닝 모델 개발
### Overhead view 사람 분류기
```java
개발 기간: 2018.07~2018.08
개발 언어: C++
피플카운팅 시스템에서의 사용 목적으로 overhead view의 객체가 사람인지 아닌지 분류하는 이진 분류기 학습
아래 사진은 검출기를 통해 검출된 영역에 대해 분류기를 적용한 결과 중 사람만 표시한 예시임
Class: 사람, Unknown
```
![overhead1](../../assets/images/overhead1.jpg){: .align-center}
![overhead2](../../assets/images/overhead2.png){: .align-center}

---

### 머리 분류기
```java
모델 학습
개발 기간: 2019.03~2019.04
개발 언어: Python
공사장 환경에서 안전모를 착용하지 않은 사람 검출 목적으로 입력된 머리를 분류하는 분류기 학습
아래 사진은 검출기를 통해 검출된 머리에 대해 분류기를 적용한 결과를 표시한 예시임
Class: 머리, 모자 쓴 머리, 안전모 쓴 머리

모델 변환
개발 기간: 2019.04~2019.04
개발 언어: Python, C++
C++ 에서 사용할 수 있도록 모델 변환 및 2가지 버전으로 DLL 작성(TensorRT, LibTorch)
```
![head1](../../assets/images/head1.jpg){: .align-center}
![head2](../../assets/images/head2.png){: .align-center}

---

### 신발 갑피 분류기
```java
개발 기간: 2017.04~2017.05
개발 언어: MATLAB
Class: 갑피 패턴1, 갑피 패턴2, 갑피 패턴3, 갑피 패턴4
```
![shoe](../../assets/images/shoe.png){: .align-center}

---

## Person Re-Identification 분야 딥러닝 모델 개발
```java
모델 학습
개발 기간: 2018.06~2018.12
개발 언어: Python
입력: 검출된 사람 이미지
출력: feature
k-reciprocal, ECN(Expanded Cross Neighborhood distance based) re-ranking 구현

모델 변환
개발 기간: 2019.01~2019.03
개발 언어: Python, C++
C++ 에서 사용할 수 있도록 모델 변환 및 2가지 버전으로 DLL 작성(TensorRT, LibTorch)
```
![ReID1](../../assets/images/ReID1.png){: .align-center}
![ReID2](../../assets/images/ReID2.png){: .align-center}

---

## 모델 변환
### 얼굴 인식 모델 변환
```java
개발 기간: 2019.07~2019.09
개발 언어: Python, C++
InsightFace PyTorch 버전(https://github.com/TreB1eN/InsightFace_Pytorch)의 얼굴 인식 모델을 C++ 에서 사용할 수 있도록 변환 및 2가지 버전으로 DLL 작성(TensorRT, LibTorch)
TensorRT에서 모델을 사용하기 위해 BatchNorm1d 연산을 C++에서 직접 구현
입력: 검출된 얼굴 이미지
출력: feature
```
![Face Recognition1](../../assets/images/Face_Recognition1.png){: .align-center}
![Face Recognition2](../../assets/images/Face_Recognition2.png){: .align-center}

---

### Pose Estimation 모델 변환
```java
모델 1
개발 기간: 2019.05~2019.06
개발 언어: Python, C++
AlphaPose PyTorch 버전(https://github.com/MVIG-SJTU/AlphaPose/tree/pytorch)의 pose estimation 모델을 C++ 에서 사용할 수 있도록 변환 및 2가지 버전으로 DLL 작성(TensorRT, LibTorch)
TensorRT에서 모델을 사용하기 위해 SE_module 수정
입력: 검출된 사람 이미지
출력: pose

모델 2
개발 기간: 2018.12~2018.12
개발 언어: C++
OpenPose의 pose estimation 모델을 별도의 빌드 없이 다른 프로젝트에서 사용하기 위해 DLL 작성
입력: 전체 프레임
출력: pose
```
![AlphaPose](../../assets/images/AlphaPose.png){: .align-center}
![OpenPose](../../assets/images/OpenPose.png){: .align-center}