# 🗃 AI SPARK 챌린지

**지역사회 대기오염 예측 인공지능 모델 개발**

</br>

## 👨‍💻 프로젝트 소개

### 2일 분량의 PM2.5 / AWS 데이터(test set)와 과거 기간의 PM2.5 / AWS 데이터 (train set)을 활용하여 3일 분량의 지역별 시간당 PM2.5 값을 예측합니다.

</br>

## 📌 주요 기능
#### ✔ PyTorch를 사용하여 시계열 데이터를 예측하는 LSTM(Long Short-Term Memory) 모델 구축
### ✔ 데이터 수집 및 전처리
- csv형식 데이터 로드 및 연도, 일시, 측정소를 기준으로 병합하여 데이터셋 생성
- 1차적으로 dropna() 메서드를 사용하여 결측치 제거
### ✔ 데이터 스케일링 및 시퀀스 생성, 데이터 분할
- StandardScaler를 사용하여 데이터 표준화 및 과거 48시간의 데이터를 기반으로 향후 72시간의 값 예측을 위한 시퀀스 생성
- 전체 데이터를 학습, 검증, 테스트 데이터로 분할(6:2:2)
### ✔ 모델 설계 및 학습
- LSTM을 활용한 RNN모델 설계(입력 시퀀스 처리로 향후 PM2.5값 예측)
- train_data로 모델을 학습시키고 val_data로 성능 평가

</br>
