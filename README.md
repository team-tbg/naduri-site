# 나드리 (Naduri) — 소개 페이지

GASOK(업비트 GIWA 체인 액셀러레이터) Phase 2 제출용 **원페이저**. GitHub Pages로 서비스한다.

🔗 **https://team-tbg.github.io/naduri-site/**

## 구성

```
index.html              페이지 전체 (자체 완결 — 외부 CSS·JS·폰트 없음)
assets/
├── flow-auth.svg       로그인부터 지갑 주소 등록까지
├── flow-deposit.svg    저금 요청부터 유동성 공급까지
├── architecture.svg    앱 · 백엔드 · GIWA 체인 3층 구조
└── yield.svg           수수료 회수와 5:5 분배 (harvest → 좌당 가치)
.nojekyll               Jekyll 처리 비활성 (정적 파일 그대로 서빙)
```

## 특징

- **자체 완결.** CDN·외부 폰트·트래커 없음. 파일만 있으면 어디서든 열린다
- **다크 모드 대응.** 페이지와 SVG가 각각 `prefers-color-scheme`를 따르고, 우상단 토글로 수동 전환도 된다
- **반응형.** 표는 가로 스크롤, 다이어그램은 `viewBox`로 축소된다

## 고칠 때

`index.html` 하나만 열면 된다. 다이어그램은 `assets/*.svg`를 직접 편집한다
(SVG 안에 자체 테마 변수가 들어 있어 페이지 CSS와 독립적으로 다크 모드가 동작한다).

로컬 확인은 파일을 브라우저로 그냥 열면 된다. 빌드 단계가 없다.

## 내용의 출처

온체인 수치(컨트랙트 주소·트랜잭션·가스)는 **GIWA Sepolia 블록 탐색기에서 직접 조회한 값**이다.
백엔드·앱 수치는 각 저장소 코드 기준.

> 원고와 배경 문서는 `team-tbg/naduri-docs`(Private)에 있다. **이 저장소는 공개**이므로
> 내부 문서(위협 모델·알려진 한계·미결 항목)를 여기에 옮기지 말 것.
