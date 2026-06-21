# Method Plan: Vehicle Trajectory Prediction

## Baseline Direction

초기 baseline은 복잡한 모델보다 입력/출력 구조와 평가 방식을 명확히 확인하는 데 초점을 둡니다.

## Possible Methods

| Method | Purpose |
| --- | --- |
| Constant velocity baseline | 가장 단순한 기준 성능 확인 |
| RNN / LSTM | 과거 trajectory sequence를 hidden state로 요약 |
| Attention-based model | 중요한 time step이나 주변 객체 정보를 선택적으로 반영 |
| Transformer-based model | sequence 전체 관계를 self-attention으로 모델링 |

## Implementation Plan

```text
1. 데이터 형식 정리
2. past / future trajectory split 정의
3. constant velocity baseline 구현
4. sequence model baseline 구현
5. ADE / FDE 등 평가 지표 정리
6. 결과와 한계 기록
```

## Notes

- 모델 성능보다 데이터 구조와 평가 setting을 먼저 고정합니다.
- 작은 baseline을 먼저 만들고 이후 모델을 확장합니다.
- 결과 수치와 해석을 분리해서 기록합니다.
