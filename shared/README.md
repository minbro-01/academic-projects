# Shared

프로젝트 간 공통으로 사용할 템플릿, 정리 형식, 유틸리티를 모아두는 공간입니다.

## Templates

| Template | Purpose |
| --- | --- |
| [`templates/project-readme.md`](./templates/project-readme.md) | 프로젝트 README 기본 구조 |
| [`templates/experiment-log.md`](./templates/experiment-log.md) | 실험 조건, 결과, 다음 실험 질문 기록 |
| [`templates/result-report.md`](./templates/result-report.md) | 최종 또는 중간 결과 보고서 정리 |

## Planned Contents

```text
shared/
├─ README.md
├─ templates/
│  ├─ project-readme.md
│  ├─ experiment-log.md
│  └─ result-report.md
└─ utils/
```

## Rule

- 여러 프로젝트에서 반복해서 쓰는 형식만 둡니다.
- 특정 프로젝트에만 필요한 코드는 각 프로젝트 폴더에 둡니다.
- 외부 코드를 사용할 경우 출처와 라이선스를 함께 남깁니다.
