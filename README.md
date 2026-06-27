# 기사 밀어내기 연구 — DB 적재 현황 대시보드

PE/비PE 부정이슈 **10개 사건**의 뉴스 수집·임베딩이 학교서버 DB(`articlepush`)에 얼마나 적재됐는지를 담당자(이니셜)별로 보여주는 정적 대시보드입니다.

- **라이브**: GitHub Pages — `https://starg-lee.github.io/articlepush-dashboard/`
- **데이터**: 회사별 기사 수 / 관련 임베딩 수(4종) / churnalism 5분류(bucket) 적재 여부
- **임베딩 4종**: bge-m3 · OpenAI text-embedding-3-large × (제목·본문 / 명사)

## 현황 (2026-06-27)
- 적재 완료(임베딩까지): **9 / 10 기업**
- 미수집: 락앤락(CSH) 1건
- bucket(5분류) 보유: 큐텐·남양유업(LGS) 2개사

## 담당자(이니셜)
PDK 고려아연·홈플러스 / CHG 롯데카드·마키노 / CSH 락앤락 / LGS 큐텐·남양유업 / KJH 오스템임플란트 / PJH bhc치킨 / SBJ DN솔루션즈

## 갱신
`index.html` 안의 `people` 배열 수치를 바꾸면 됩니다(DB 카운트 반영). 외부 의존성 없는 단일 HTML 파일.
