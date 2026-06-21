# Method Plan: Road Topology & Ego-lane Inference

## Method Direction

도로 이미지를 단순히 분류하는 것이 아니라, 차선과 도로 구조를 인식하고 그 구조를 바탕으로 ego-lane을 추론하는 흐름을 정리합니다.

## Possible Pipeline

```text
1. 입력 이미지 또는 scene 정의
2. 차선/도로 구조 인식
3. road topology representation 구성
4. ego vehicle 위치와 road structure 관계 정리
5. ego-lane candidate 추론
6. 실패 사례와 한계 분석
```

## Representation Candidates

| Representation | Purpose |
| --- | --- |
| Lane mask | 차선 영역을 segmentation 형태로 표현 |
| Lane graph | 차선 간 연결 관계를 graph로 표현 |
| Topology label | 교차로, 합류, 분기 등 구조를 label로 표현 |
| Evidence map | 모델이 판단에 사용한 근거를 시각화 |

## Notes

- 처음부터 복잡한 모델을 만들기보다, 문제 표현과 평가 기준을 먼저 명확히 합니다.
- 모델 출력과 추론 근거를 분리해서 기록합니다.
- 실패 사례는 프로젝트의 중요한 결과로 남깁니다.
