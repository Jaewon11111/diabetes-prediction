# 🩺 Diabetes Prediction with Clinical Insights and Machine Learning

본 프로젝트는 당뇨병 예측을 위한 머신러닝 모델(Logistic Regression, Random Forest)을 구축하고,  
모델 성능 평가 지표를 비교하고 변수 중요도를 분석하여 성능 차이를 설명한 보고서 기반 데이터 분석 프로젝트입니다.

> 📄 **[최종 보고서 PDF 보기](./Diabetes_Prediction_Report.pdf)**  
> 💻 **[분석 코드 (Jupyter Notebook)](./Diabetes_Prediction.ipynb)**

---

## 📌 프로젝트 개요

- **데이터 출처**: [Kaggle - Diabetes Data Set](https://www.kaggle.com/datasets/mathchi/diabetes-data-set)
- **목표**:  
  - 데이터셋의 독립변수와 당뇨 발생 간의 연관성 분석  
  - 의료 도메인 지식 기반 변수 전처리 및 이상치 처리  
  - 두 가지 모델(Logistic Regression, Random Forest)을 적용하여 성능 비교  
  - 모델별 변수 중요도를 기반으로 성능 차이 해석

---

## 🔍 주요 분석 과정

1. **의학적 변수 정의 및 전처리 기준 도출**

2. **데이터 전처리**  
   - 이상치 제거 및 평균·중앙값 대체  
   - 로그 변환 및 스케일링(StandardScaler)  
   - 다중공선성 점검 (VIF 분석)

3. **모델링 및 성능 비교**  
   - `Logistic Regression`, `Random Forest` 모델 학습  
   - Confusion Matrix, F1 Score, ROC-AUC 기반 비교

4. **결론**

  - ROC-AUC 기준 두 모델 모두 우수  
  - 정확도와 F1 Score, ROC-AUC에서 로지스틱 회귀가 약간 우세하나 재현율 측면에서는 랜덤 포레스트가 조금 더 우세  
  - Pregnancies 변수의 반영 정도가 랜덤 포레스트 모델의 재현율이 높게 나타난 원인일 가능성이 있음

---

## 🧠 결과 요약

| 모델                  | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|-----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression   | 0.819    | 0.698     | 0.682  | 0.690    | 0.873   |
| Random Forest         | 0.805    | 0.660     | 0.705  | 0.681    | 0.861   |

- 지표별 성능 비교 요약:
  - Logistic Regression: Accuracy, Precision, F1 Score, ROC-AUC 우세
  - Random Forest: Recall 우세

---

## 🛠 사용 기술

- Python (Pandas, NumPy, Seaborn, Scikit-learn)
- Jupyter Notebook
- Medical domain knowledge-based data cleansing
- PDF Report 작성 (근거 기반 의학 정보 인용 포함)

---

## 👩‍⚕️ 작성자

- Interests: 헬스케어, 의료 AI, 데이터 기반 의학적 의사결정, MSL/MA 직무 등  
- Contact: [www.linkedin.com/in/재원-박-1638aa31a](https://www.linkedin.com/in/재원-박-1638aa31a)

---

## 📎 참고 자료

- [서울아산병원 건강정보](https://www.amc.seoul.kr/)
- [대한당뇨병학회](https://www.diabetes.or.kr/)
- [질병관리청 건강정보 등](https://health.kdca.go.kr/)
