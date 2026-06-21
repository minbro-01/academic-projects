# Experiment Plan: Vehicle Trajectory Prediction

## Evaluation Goal

예측 모델이 주변 차량의 미래 위치를 얼마나 정확하게 예측하는지 확인합니다.

## Metrics To Consider

| Metric | Meaning |
| --- | --- |
| ADE | 전체 예측 구간에서 평균 위치 오차 |
| FDE | 마지막 예측 시점의 위치 오차 |
| Miss Rate | 일정 threshold 이상 벗어난 예측 비율 |

## Experiment Table

| Experiment | Model | Input | Metric | Status |
| --- | --- | --- | --- | --- |
| E01 | Constant velocity baseline | Past trajectory | ADE / FDE | Planned |
| E02 | RNN baseline | Past trajectory | ADE / FDE | Planned |
| E03 | Attention-based model | Past trajectory + context | ADE / FDE | Planned |

## Record Rule

- 데이터 split 기준을 함께 남깁니다.
- 같은 metric이라도 prediction horizon이 다르면 구분합니다.
- 결과가 좋지 않아도 원인과 다음 실험 질문을 기록합니다.
