# Machine Learning 실습 (2026-11-13)

M애플리케이션배포의 Machine Learning 실습파일 제출 과제입니다.

- machine_learning_practice.ipynb: 설명, 코드, 그래프와 실제 실행 결과를 포함합니다.
- requirements.txt: 검증한 라이브러리 버전입니다.

## 실행

Python 3.12 이상에서 가상환경을 만든 다음 실행합니다.

```sh
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyter notebook machine_learning_practice.ipynb
```

커널을 다시 시작하고 모든 셀을 순서대로 실행합니다. Iris는 내장 데이터이며 엑셀의 수치 예제는 셀 안에 포함되어 별도 데이터 파일 없이 실행됩니다.

## 실습 내용

Iris EDA, 결정 트리, GridSearchCV, Random Forest, XGBoost, LightGBM, KNN, Optuna 50회 탐색, 최종 테스트, 혼동행렬, 임계값, ROC AUC, PR/AP, 거리 계산, Gini, Log loss, 공분산과 상관계수, SGD, L1/L2 규제를 포함합니다.

모델 선택은 학습 120개 자료의 5-fold 교차검증으로 수행하고 보관한 테스트 30개를 마지막에 평가합니다. 실행 검증 결과 Optuna Random Forest의 테스트 정확도는 29/30(96.67%)였습니다. 작은 예제 데이터의 결과이며 실행 시간은 환경에 따라 달라집니다.

참고 자료와 수식의 경계 조건은 노트북에 명시했습니다.

학교 과제: https://eclass.kbu.ac.kr/mod/assign/view.php?id=500974
