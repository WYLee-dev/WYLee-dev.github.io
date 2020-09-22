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
last_modified_at: '2020-09-22 00:00:00 +0800'
---

## Instance Segmentation 분야 딥러닝 모델 개발
### 0. Instance Segmentation 모델 학습 데이터 태깅 툴 개발
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

### 1. 토마토 인식을 위한 딥러닝 기반 Instance Segmentation 모델 학습
<!-- PyTorch를 이용하여 학습한 모델을 ONNX로 변환한 뒤 ONNX Runtime을 이용하여 C++에서 사용하였음 -->
<!-- 모델: Mask R-CNN(backbone: ResNet50-FPN) -->
> [demo video link](https://youtu.be/ewgW1aQRRyk)


```java
개발 기간: 2020.04~2020.06
개발 언어: Python
인식 대상 토마토: 실제 농장 환경에서 수확 로봇의 워크스페이스에 포함되는 토마토
Class: 숙도 1(USDA 숙도 6단계 중 Green, Breaker), 숙도 2(USDA 숙도 6단계 중 Green, Breaker), 숙도 3(USDA 숙도 6단계 중 Green, Breaker)
```
![tomato1](../../assets/images/tomato1.jpg){: .align-center}
![tomato2](../../assets/images/tomato2.jpg){: .align-center}

## Object Detection 분야 딥러닝 모델 개발
### 1. 마스크 검출기
<!-- 마스크 검출기와 tracker를 이용하여 불량 마스크 분류 시스템 개발 -->
<!-- 모델: YOLOv4 -->
>[article link1](http://naver.me/xBDFbMHS) [article link2](http://naver.me/xN9fk3cb)


```java
개발 기간: 2020.08~2020.08
개발 언어: C++
Class: 마스크(양품), 마스크(불량품)
```
![mask1](../../assets/images/mask1.png){: .align-center}
![mask2](../../assets/images/mask2.png){: .align-center}

### 2. 일반 객체 검출기
<!-- 모델: YOLOv3, MobileNetV2-SSD -->
```java
개발 기간: 2019.08~2019.10
개발 언어: C++, Python
Class: 사람, 차량, 트럭, 버스, 휠체어, 유모차, 불꽃
```
![object1](../../assets/images/object1.jpg){: .align-center}
![object2](../../assets/images/object2.jpg){: .align-center}

### 3. 얼굴 검출기
<!-- 얼굴 인식 시스템에서의 사용 목적으로 얼굴 검출기 학습 -->
<!-- 모델: YOLOv3, YOLOv3-tiny -->
```java
개발 기간: 2019.04~2019.06
개발 언어: C++
Class: 얼굴
```
![face1](../../assets/images/face1.jpg){: .align-center}
![face2](../../assets/images/face2.jpg){: .align-center}

### 4. 사람 검출기
<!-- 모델: YOLOv3 -->
```java
개발 기간: 2019.01~2019.02
개발 언어: C++
Class: 아이(미취학아동), 어른(아이에 해당하지 않는 사람)
```
![person1](../../assets/images/person1.jpg){: .align-center}
![person2](../../assets/images/person2.jpg){: .align-center}

## Classification 분야 딥러닝 모델 개발

## Person Re-Identification 분야 딥러닝 모델 개발

## 모델 변환