# Problem Definition: Vehicle Trajectory Prediction

## Problem

주변 차량의 과거 위치와 움직임 정보를 바탕으로 이후의 궤적을 예측하는 문제를 다룹니다.

자율주행 시스템에서는 주변 객체가 앞으로 어디로 이동할지 예측해야 안전한 판단과 계획이 가능하므로, trajectory prediction은 perception과 planning 사이를 연결하는 중요한 문제입니다.

## Input

```text
- Past trajectory of surrounding vehicles
- Ego vehicle state, if available
- Road context, if available
- Time step information
```

## Output

```text
- Future trajectory points
- Prediction horizon
- Optional uncertainty or confidence
```

## Key Questions

- 과거 trajectory를 어떤 sequence 형태로 표현할 것인가?
- RNN, attention, Transformer 중 어떤 구조가 이 문제에 적합한가?
- 예측 결과를 어떤 metric으로 평가할 것인가?
- 단순 위치 오차 외에 실제 주행 관점에서 의미 있는 평가는 무엇인가?

## Related Study Notes

- [`ai-engineering-study/coursework/deep-learning`](https://github.com/minbro-01/ai-engineering-study/tree/main/coursework/deep-learning)
- [`ai-engineering-study/coursework/time-series-analysis`](https://github.com/minbro-01/ai-engineering-study/tree/main/coursework/time-series-analysis)
