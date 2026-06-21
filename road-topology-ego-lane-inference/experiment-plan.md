# Experiment Plan: Road Topology & Ego-lane Inference

## Evaluation Goal

도로 topology 인식과 ego-lane 판단이 실제로 어떤 상황에서 잘 되고, 어떤 상황에서 실패하는지 확인합니다.

## Evaluation Points

| Point | Question |
| --- | --- |
| Topology recognition | 도로 구조를 올바르게 인식했는가? |
| Ego-lane inference | ego 차량의 차선을 올바르게 판단했는가? |
| Evidence quality | 판단 근거를 설명할 수 있는가? |
| Failure case | 교차로, 합류, 혼잡 차선에서 어떤 문제가 생기는가? |

## Experiment Table

| Experiment | Input | Method | Metric / Check | Status |
| --- | --- | --- | --- | --- |
| E01 | Simple lane scene | Rule or baseline model | qualitative check | Planned |
| E02 | Intersection scene | topology representation | ego-lane correctness | Planned |
| E03 | Congested lane scene | model + evidence | failure analysis | Planned |

## Record Rule

- 성공 사례보다 실패 사례를 자세히 남깁니다.
- 인식 결과와 추론 결과를 분리해서 기록합니다.
- 판단 근거가 부족한 경우 한계로 표시합니다.
