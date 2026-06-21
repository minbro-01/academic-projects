# Road Topology & Ego-lane Inference

도로 topology를 인식하고, 인식한 근거를 바탕으로 ego 차량의 차선을 판단하는 프로젝트 공간입니다.

## Problem

교차로와 차선 혼잡 구간에서는 단순 차선 검출만으로 ego 차량의 주행 차선을 판단하기 어렵습니다. 이 프로젝트는 도로 구조와 주변 차선 관계를 함께 인식하고, 그 근거를 바탕으로 ego-lane을 추론하는 문제를 다룹니다.

## Project Goal

- 도로 topology와 ego-lane 판단 문제를 정의합니다.
- 컴퓨터 비전 기반 인식 결과를 구조화하는 방법을 정리합니다.
- 모델이 인식한 근거를 바탕으로 추론하는 흐름을 기록합니다.
- 구현, 실험, 결과, 한계를 프로젝트 문서로 남깁니다.

## Documents

| Document | Purpose |
| --- | --- |
| [`problem-definition.md`](./problem-definition.md) | 문제 정의, 입력/출력, 핵심 질문 정리 |
| [`method-plan.md`](./method-plan.md) | road topology 표현과 ego-lane 추론 흐름 정리 |
| [`experiment-plan.md`](./experiment-plan.md) | 평가 기준, 실험 계획, 실패 사례 기록 방식 정리 |

## Related Study Notes

컴퓨터 비전 개념 정리는 [`ai-engineering-study/coursework/computer-vision`](https://github.com/minbro-01/ai-engineering-study/tree/main/coursework/computer-vision)에 기록합니다.

## Planned Structure

```text
road-topology-ego-lane-inference/
├─ README.md
├─ problem-definition.md
├─ method-plan.md
├─ experiment-plan.md
├─ data/
├─ notebooks/
├─ src/
├─ results/
└─ report.md
```

## Status

To be organized
