# 건설용 자갈 암석 종류 분류 AI 경진대회 🪨

## 📋 대회 정보
- **대회명**: 건설용 자갈 암석 종류 분류 AI 경진대회
- **주최**: 데이콘
- **후원**: 한국지능정보사회진흥원(NIA)
- **대회 링크**: [https://dacon.io/competitions/official/236471/overview/description](https://dacon.io/competitions/official/236471/overview/description)
- **시작일**: 2025-04-08
- **마감일**: 2025-05-30
- **평가 지표**: Macro F1 Score
- **문제 유형**: 이미지 분류 (Computer Vision)

## 🎯 대회 목표
건설용 자갈의 이미지를 기반으로 암석 종류를 자동으로 분류하는 AI 알고리즘을 개발하여, 건설 현장의 품질 검사 자동화와 디지털 전환에 기여하는 것이 목표입니다.

## 📊 데이터 개요

### 데이터 구조
- **훈련 데이터**: 7개 클래스, 총 380,020장의 PNG 이미지
- **테스트 데이터**: 95,006장의 PNG 이미지
- **클래스 수**: 7개 (구체적인 클래스명은 데이터 확인 필요)

### 파일 구조
```
train/
├── Andesite/     # 클래스별 폴더
├── Basalt/
├──  Weathered_Rock/
├── Gneiss/
├── Grantite/
├── Mud_Sandstone/
└── Etc/

test/             # 평가용 이미지들

test.csv          # 테스트 데이터 정보
├── ID: 평가 샘플 고유 ID
└── img_path: 이미지 파일 경로

sample_submission.csv  # 제출 양식
├── ID: 평가 샘플 고유 ID
└── rock_type: 예측한 암석 종류 클래스
```

## 🚀 진행 상황


### 📈 단계별 진행 상황

#### 1단계: 데이터 탐색 및 이해 ⏳
- [ V ] 대회 데이터셋 다운로드 및 구조 파악
- [ V ] 7개 클래스별 이미지 분포 분석
- [ ] 이미지 품질 및 특성 파악
- [ ] 탐색적 데이터 분석(EDA) 노트북 작성

#### 2단계: 데이터 전처리 ⏳
- [ ] 이미지 크기 통일 및 정규화
- [ ] 데이터 증강 기법 적용
- [ ] 클래스 불균형 문제 해결 방안 수립
- [ ] 전처리 파이프라인 구축

#### 3단계: 모델링 ⏳
- [ ] 베이스라인 모델 구현 (Inception ResNet)
- [ ] 최신 아키텍처 실험 (ConvNeXt, EfficientNet)
- [ ] Vision Transformer 모델 시도
- [ ] 앙상블 방법 적용

#### 4단계: 평가 및 개선 ⏳
- [ ] 교차 검증을 통한 성능 평가
- [ ] 오버피팅/언더피팅 분석
- [ ] 모델 해석 및 특성 중요도 분석
- [ ] 성능 개선 방안 도출

## 🏆 성과 지표

### 현재 최고 성과
- **모델**: 아직 없음
- **성능**: 아직 없음
- **제출일**: 아직 없음

### 성과 변화 추이
| 날짜 | 모델 | 성능 | 개선사항 |
|------|------|------|----------|
| - | - | - | - |

## 💡 주요 인사이트

### 데이터 분석 결과
- **이미지 수**: 훈련 380,020장, 테스트 95,006장
- **클래스 수**: 7개 (균형잡힌 분포 여부 확인 필요)
- **이미지 형식**: PNG 파일

### 모델링 인사이트
- **베이스라인**: Inception ResNet 활용 가능
- **최신 트렌드**: ConvNeXt, EfficientNet, Vision Transformer
- **핵심 기법**: Negative Sampling, 앙상블, 데이터 증강

## 🔧 사용할 기술 및 라이브러리

### 데이터 처리
- **이미지 처리**: OpenCV, PIL, albumentations
- **데이터 관리**: pandas, numpy

### 시각화
- **이미지 시각화**: matplotlib, seaborn
- **데이터 분석**: plotly

### 머신러닝/딥러닝
- **딥러닝 프레임워크**: PyTorch
- **전이학습**: torchvision.models
- **최적화**: torch.optim, torch.optim.lr_scheduler

### 모델 아키텍처
- **CNN 기반**: ResNet, EfficientNet, ConvNeXt
- **Transformer 기반**: Vision Transformer (ViT)
- **앙상블**: 모델 조합 및 앙상블

## 📚 참고 자료

### 코드 공유 분석
- **1위**: SFAI (구체적 방법론 미공개)
- **2위**: InternImage + Negative Sampling (0.93306)
- **3위**: ConvNeXt
- **베이스라인**: Inception ResNet

### 논문 및 문서
- [ConvNeXt: A ConvNet for the 2020s](https://arxiv.org/abs/2201.03545)
- [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](https://arxiv.org/abs/1905.11946)
- [Vision Transformer (ViT)](https://arxiv.org/abs/2010.11929)

### 커뮤니티
- [데이콘 대회 페이지](https://dacon.io/competitions/official/236471/overview/description)
- [데이콘 코드 공유](https://dacon.io/competitions/official/236471/codeshare)


## 📝 학습 노트

### 새로 배운 개념
- **자갈 암석 분류**: 건설업계의 실제 문제와 AI 적용
- **Macro F1 Score**: 다중 클래스 분류에서의 평가 지표

### 어려웠던 점과 해결 방법
- 아직 진행 중...

### 개선하고 싶은 점
- 체계적인 실험 기록 시스템 구축
- 다양한 모델 아키텍처 실험 경험

## 🚨 주의사항

### 데이터 관리
- **이미지 크기**: 대용량 이미지 데이터 처리 시 메모리 관리 주의
- **클래스 불균형**: 7개 클래스 간 데이터 분포 확인 필요
- **이미지 품질**: 현장 촬영 환경에 따른 품질 차이 고려

### 모델링 고려사항
- **전이학습**: 사전 훈련된 모델 활용 시 이미지 크기 및 전처리 방법 통일
- **데이터 증강**: 자갈 이미지의 특성을 고려한 증강 기법 선택
- **앙상블**: 다양한 모델의 장점을 결합한 최적 조합 찾기