# 👗 Fashion MNIST Classification

패션 아이템 이미지를 CNN 딥러닝 모델로 분류하는 웹 애플리케이션입니다.

---

## 📌 프로젝트 소개

Fashion MNIST 데이터셋을 기반으로 학습된 CNN 모델을 활용하여, 사용자가 업로드한 패션 아이템 이미지를 10가지 카테고리로 분류합니다. Streamlit을 통해 간편한 웹 인터페이스를 제공합니다.

---

## 🗂️ 분류 카테고리

| 번호 | 한국어 | English |
|------|--------|---------|
| 0 | 티셔츠/톱 | T-shirt/top |
| 1 | 바지 | Trouser |
| 2 | 풀오버 | Pullover |
| 3 | 드레스 | Dress |
| 4 | 코트 | Coat |
| 5 | 샌들 | Sandal |
| 6 | 와이셔츠 | Shirt |
| 7 | 스니커즈 | Sneaker |
| 8 | 가방 | Bag |
| 9 | 앵클부츠 | Ankle boot |

---

## 📁 파일 구조

```
fashion_mnist_classification/
├── app.py                  # Streamlit 웹 애플리케이션
├── model.py                # 모델 로드 및 예측 함수
├── model_cnn_final.keras   # 학습된 CNN 모델 파일
├── requirements.txt        # 의존성 패키지 목록
└── README.md
```

---

## ⚙️ 설치 및 실행

### 1. 패키지 설치

```bash
pip install -r requirements.txt
```

### 2. 앱 실행

```bash
streamlit run app.py
```

---

## 🛠️ 기술 스택

| 분류 | 기술 |
|------|------|
| 딥러닝 프레임워크 | TensorFlow >= 2.20.0, Keras 3.10.0 |
| 웹 프레임워크 | Streamlit 1.49.1 |
| 이미지 처리 | Pillow 11.3.0 |
| 시각화 | Matplotlib 3.10.0 |

---

## 🔍 동작 방식

1. 사용자가 패션 아이템 이미지를 업로드
2. 이미지를 **28x28 흑백(그레이스케일)** 으로 변환 및 정규화
3. 학습된 CNN 모델(`model_cnn_final.keras`)로 예측 수행
4. 10개 카테고리에 대한 **확률값을 내림차순으로 정렬**하여 결과 출력

---

## 📋 요구사항

```
streamlit==1.49.1
tensorflow>=2.20.0
keras==3.10.0
Pillow==11.3.0
matplotlib==3.10.0
```
