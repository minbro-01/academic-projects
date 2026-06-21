# Problem Definition: Road Topology & Ego-lane Inference

## Problem

교차로와 차선 혼잡 구간에서는 단순한 차선 검출만으로 ego 차량이 어느 차선에 있는지 판단하기 어렵습니다.

이 프로젝트는 도로 topology를 인식하고, 모델이 인식한 근거를 바탕으로 ego 차량의 차선을 추론하는 문제를 다룹니다.

## Input

```text
- Road image or driving scene input
- Lane / road structure information, if available
- Ego vehicle position or camera perspective
- Optional map or topology prior
```

## Output

```text
- Recognized road topology
- Candidate lane structure
- Ego-lane inference result
- Reasoning evidence or intermediate representation
```

## Key Questions

- 차선 혼잡 구간에서 road topology를 어떻게 표현할 것인가?
- 모델이 인식한 근거를 사람이 이해 가능한 형태로 정리할 수 있는가?
- 단순 lane detection과 ego-lane inference는 무엇이 다른가?
- 교차로처럼 차선 구조가 복잡한 상황에서 어떤 실패 사례가 생기는가?

## Related Study Notes

- [`ai-engineering-study/coursework/computer-vision`](https://github.com/minbro-01/ai-engineering-study/tree/main/coursework/computer-vision)
