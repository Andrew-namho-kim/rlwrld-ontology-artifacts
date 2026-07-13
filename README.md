# RLWRLD Ontology — Artifacts

RLWRLD 온톨로지 프로젝트의 시각화 산출물(자체 완결형 HTML)입니다.

| 파일 | 내용 |
|------|------|
| [`index.html`](index.html) | 랜딩 페이지 (전체 목록) |
| [`knowledge-graph.html`](knowledge-graph.html) | 지식 그래프 — 도메인별 노드·관계 인터랙티브 뷰 |
| [`data-logic-action.html`](data-logic-action.html) | Data · Logic · Action 계층 구조 |
| [`overview.html`](overview.html) | 프로젝트 개요 |
| [`data-lake.html`](data-lake.html) | Data Lake — 소스→주기→클래스→인스턴스 계보 (선언 feeds vs 실제 provenance) |
| [`lineage-flow.html`](lineage-flow.html) | Lineage Flow — 원 시스템→소스→클래스→인스턴스 유입 구조 좌→우 흐름도 (팬/줌) |
| [`bsp-product-map.html`](bsp-product-map.html) | BSP Product Map — 26년 하반기 BSP OS 프로덕트 간트 (세부 기능 × 기간, 상태 인코딩 막대) |

각 HTML은 외부 의존성이 없어 그대로 열면 렌더됩니다. `data-lake.html`·`lineage-flow.html`의 데이터는 `tools/build_datalake_data.py`가 `20_schema/`·`30_instances/`를 읽어 두 페이지에 임베드하므로, 소스/인스턴스가 바뀌면 이 스크립트를 다시 실행한 뒤 커밋하세요.

## GitHub Pages 배포

`main` 브랜치 push 후 저장소 **Settings → Pages → Source: `main` / `root`** 로 설정하면 다음 URL로 공개됩니다.

```
https://<GitHub사용자명>.github.io/<저장소명>/
https://<GitHub사용자명>.github.io/<저장소명>/knowledge-graph.html
```

## 노션 임베드

노션 페이지에서 `/embed` → 위 Pages URL 붙여넣기 → 인터랙티브 그래프가 인라인으로 렌더됩니다.
