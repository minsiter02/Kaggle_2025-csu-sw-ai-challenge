# 2025 CSU SW AI Challenge - 7조

본 저장소는 [2025 CSU SW AI Challenge](https://www.kaggle.com/competitions/2025-csu-sw-ai-challenge)에 참여한 **7조**의 최종 솔루션과 실험 과정을 담고 있습니다.

## 1\. 대회 개요 (Overview)

  - **대회 목표**: 각 이미지에 대해 픽셀 단위 균열 확률/마스크를 예측
  - **데이터**: [사용한 데이터의 특징을 간략히 설명합니다.]
  - **평가 지표**: Dice F-beta (β=2.0) 를 사용
β=2.0은 재현율(Recall) 에 더 큰 가중치를 부여하여, 균열 픽셀을 놓치지 않는 능력을 강조
Metric 구현은 Kaggle에서 공식 제공하는 Dice F-beta를 따르며, 제출 마스크/확률을 기준으로 대회 평가 스크립트가 일괄 계산
## 2\. 사용 방법 (How to Reproduce)

### 2.1. 환경 설정

1.  **저장소 복제 (Clone Repository)**

    ```bash
    git clone https://github.com/minsiter02/Kaggle_2025-csu-sw-ai-challenge.git
    cd Kaggle_2025-csu-sw-ai-challenge
    ```

2.  **필요 라이브러리 설치 (Install Dependencies)**

    ```bash
    pip install -r requirements.txt
    ```

3.  **데이터 준비 (Data Setup)**
    [Kaggle 대회 페이지](https://www.kaggle.com/competitions/2025-csu-sw-ai-challenge/data)에서 데이터를 다운로드 받은 후, `input/` 폴더 안에 위치시킵니다.

    ```
    input/2025-csu-sw-ai-challenge/archive/
    ├
    ├── train/
    ├── test/
    ├── val/
    └── sample_submission.csv
    ```

### 2.2. 실행

아래의 Jupyter Notebook 파일을 순서대로 실행하여 전체 과정을 재현할 수 있습니다.

1.  **`baseline-crack-seg.ipynb.ipynb`**

      - 학습 및 제출 파일 생성을 진행합니다.


## 3\. 솔루션 요약 (Solution Summary)

### 3.1. 데이터 분석 및 특징 공학

  - [가장 중요했던 변수나 파생 변수에 대해 간략히 서술합니다.]
  - [결측치 처리, 인코딩 등 주요 전처리 기법을 요약합니다.]

### 3.2. 모델링

  - **사용한 모델**: [예: LightGBM, XGBoost, CatBoost 등]
  - **주요 하이퍼파라미터**: [핵심적인 하이퍼파라미터 값이나 튜닝 방식을 기입합니다.]
  - **검증 전략**: [예: 5-Fold Stratified K-Fold Cross Validation]

## 4\. 최종 결과 (Result)

| Score Type   | Score  |
| :----------- | :----- |
| Public Score | [점수] |
| Private Score| [점수] |

-----