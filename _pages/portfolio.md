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
last_modified_at: '2020-09-21 00:00:00 +0800'
---

## Instance Segmentation 분야 딥러닝 모델 개발
### Instance Segmentation 모델 학습 데이터 태깅 툴 개발
[github link](https://github.com/KITECH-AI-LAB/InstanceSegmentationAnnotationTool)
```java
개발 기간
ver 1.0: 2020.03~2020.04
ver 1.1: 2020.08~2020.09
개발 언어: C++(Qt, OpenCV)
입력: 이미지
출력: *.mask: 입력 이미지와 같은 해상도의 mask, *.txt: *.mask에 대한 label, *.dat: mask 생성을 위한 마커(실제 모델 학습에는 필요 없음)
```
![ISAT](https://user-images.githubusercontent.com/68308047/92673434-0da6e580-f356-11ea-9dee-7a3dc59d0ac8.png){: .align-center}

### 토마토 인식을 위한 딥러닝 기반 Instance Segmentation 모델 학습
[video link](https://youtu.be/ewgW1aQRRyk)
```java
개발 기간: 2020.04~2020.06
개발 언어: Python(PyTorch)
모델: Mask R-CNN(backbone: ResNet50-FPN)
인식 대상 토마토: 실제 농장 환경에서 수확 로봇의 워크스페이스에 포함되는 토마토
PyTorch를 이용하여 학습한 모델을 ONNX로 변환한 뒤 ONNX Runtime을 이용하여 C++에서 사용하였음
Class: 숙도 1(USDA 숙도 6단계 중 Green, Breaker), 숙도 2(USDA 숙도 6단계 중 Green, Breaker), 숙도 3(USDA 숙도 6단계 중 Green, Breaker)
```
![tomato](../../assets/images/tomato.png){: .align-center}

## Object Detection 분야 딥러닝 모델 개발
### 마스크 검출기
```java
개발 기간: 2020.08~2020.08
개발 언어: C++(Darknet)
모델: YOLOv4
마스크 불량 인식 시스템에서의 사용 목적으로 마스크 검출기 학습
Class: 양품, 불량품
```
[기사1](http://naver.me/xBDFbMHS)
[기사2](http://naver.me/xN9fk3cb)

### 사람 검출기
```java
개발 기간: 20xx.xx~20xx.xx
개발 언어: C++(Darknet)
모델: YOLOv3
어린이집 아동학대 의심 상황 검출 목적으로 실내 환경에서의 사람 검출기 학습
Class: 아이(미취학아동), 어른(아이에 해당하지 않는 사람)
```
![person1](https://user-images.githubusercontent.com/54341546/65399022-6e5faa00-ddf5-11e9-9bbe-6e163cdf0960.jpg){: .align-center}
![person2](https://user-images.githubusercontent.com/54341546/65399028-73245e00-ddf5-11e9-9b00-26c6cc97aed3.jpg){: .align-center}

### 얼굴 검출기
```java
개발 기간: 20xx.xx~20xx.xx
개발 언어: C++(Darknet)
모델: YOLOv3, YOLOv3-tiny
얼굴 인식 시스템에서의 사용 목적으로 얼굴 검출기 학습
Class: 얼굴
```
![face1](https://user-images.githubusercontent.com/54341546/65397060-bc6db100-dde7-11e9-8ea0-dba59d474374.jpg){: .align-center}
![face2](https://user-images.githubusercontent.com/54341546/65397062-bd9ede00-dde7-11e9-97d1-73001344b829.jpg){: .align-center}

### 일반 객체 검출기
```java
개발 기간: 20xx.xx~20xx.xx
개발 언어: C++(Darknet), Python(TensorFlow)
모델: YOLOv3, MobileNetV2-SSD
Class: 사람, 차량, 트럭, 버스, 휠체어, 유모차, 불꽃
```
![face1](https://user-images.githubusercontent.com/54341546/65396696-f8067c00-dde3-11e9-8154-67a4225acfca.jpg){: .align-center}
![face2](https://user-images.githubusercontent.com/54341546/65396701-06ed2e80-dde4-11e9-9ec7-e449d6d7d6b0.jpg){: .align-center}

## Classification 분야 딥러닝 모델 개발

## Person Re-Identification 분야 딥러닝 모델 개발

## 모델 변환