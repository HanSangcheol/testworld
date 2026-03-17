# 🌟 TestWorld 프로젝트 매니페스트
> 새 테스트 추가 또는 기존 테스트 수정 시 **반드시 이 파일을 먼저 읽고, 작업 후 업데이트**할 것

---

## 📁 파일 목록 (배포 기준)

| 파일명 | 상태 | 설명 |
|---|---|---|
| `index.html` | ✅ 활성 | 홈 페이지 |
| `love-style-test.html` | ✅ 활성 | 나의 연애 스타일 테스트 |
| `animal-test.html` | ✅ 활성 | 나를 동물로 표현하면? |
| `past-life-test.html` | ✅ 활성 | 나의 전생은? |
| `talent-test.html` | ✅ 활성 | 숨겨진 재능 테스트 |
| `hell-test.html` | ✅ 활성 | 당신의 지옥은? |
| `privacy.html` | ✅ 활성 | 개인정보처리방침 |

---

## 🧪 테스트 상세 정보

### 1. love-style-test.html — 나의 연애 스타일은?
- **유형 수**: 8가지 (A~H)
- **문항 수**: 20문항
- **소요시간**: 약 3분
- **결과 유형**: A(로맨틱 드리머), B(열정 표현형), C(안정 배려형), D(자유 독립형), E(열정 낭만형), F(활동 표현형), G(균형 조율형), H(내면 탐구형)
- **scores 초기화**: `{ A:0, B:0, C:0, D:0, E:0, F:0, G:0, H:0 }`
- **다국어**: KO / EN ✅
- **더보기 링크**: past-life, animal, talent

### 2. animal-test.html — 나를 동물로 표현하면?
- **유형 수**: 확인 필요 (동물 종류 수)
- **소요시간**: 약 3분
- **다국어**: KO / EN ✅
- **더보기 링크**: love-style, past-life, talent

### 3. past-life-test.html — 나의 전생은?
- **유형 수**: 4가지
- **문항 수**: 16문항
- **소요시간**: 약 2~3분
- **다국어**: KO / EN ✅
- **더보기 링크**: love-style, animal, talent (class="test-item" 사용 — 다른 파일과 클래스명 다름, 기능 정상)

### 4. talent-test.html — 숨겨진 재능 테스트
- **소요시간**: 약 3분
- **다국어**: KO / EN ✅
- **더보기 링크**: love-style, animal, past-life, hell

### 5. hell-test.html — 당신의 지옥은?
- **유형 수**: 7가지 (A~G)
- **문항 수**: 15문항
- **소요시간**: 약 2분
- **결과 유형**: A(혼돈의 지옥), B(연결 강요의 지옥), C(노력 무효의 지옥), D(고독의 지옥), E(판단의 지옥), F(영원한 반복의 지옥)
- **scores 초기화**: `{ A:0, B:0, C:0, D:0, E:0, F:0, G:0 }`
- **다국어**: KO / EN ✅
- **더보기 링크**: love-style, animal, past-life, talent

---

## 🔗 연동 규칙 (새 테스트 추가 시 필수 체크리스트)

### ✅ 새 테스트 파일 생성 시
- [ ] `index.html` → 테스트 카드 추가 (featured-card 또는 test-grid)
- [ ] `index.html` → KO/EN 번역 데이터 추가 (`ui.ko`, `ui.en` 객체)
- [ ] `index.html` → 히어로 스탯 업데이트 (테스트 수, 결과 유형 수)
- [ ] **기존 활성 테스트 전체** → 더보기(more-item / test-item) 섹션에 새 테스트 링크 추가
- [ ] 새 테스트 파일 → 더보기 섹션에 **기존 활성 테스트 전체** 링크 포함
- [ ] 새 테스트 파일 → footer에 `index.html` 홈 링크 포함
- [ ] 새 테스트 파일 → footer 저작권 연도 **2026** 확인
- [ ] 새 테스트 파일 → AdSense 태그 `ca-pub-XXXXXXXXXXXXXXXX` 포함
- [ ] TESTWORLD_MANIFEST.md 업데이트 (파일 목록, 테스트 상세, 변경 이력)

### ✅ 기존 테스트 수정 시
- [ ] `index.html` 카드 정보 동기화 (문항 수, 소요시간, 유형 수)
- [ ] KO/EN 번역 데이터 키 일치 확인
- [ ] `toggleLang()` 내 변수 중복 선언 없는지 확인
- [ ] HTML `id` 중복 선언 없는지 확인
- [ ] `scores` 초기화 키가 실제 유형 A~? 와 일치하는지 확인

---

## ⚠️ 알려진 특이사항 (함정 주의)

| 파일 | 특이사항 |
|---|---|
| `past-life-test.html` | 더보기 링크 클래스명이 `test-item` (다른 파일은 `more-item`) — 기능 동일, 혼동 주의 |
| `love-style-test.html` | scores 초기화 키가 A~H 8개 — D까지만 쓰면 유형 E~H 점수 누락됨 |
| `hell-test.html` | 일부 선택지에 음수 점수(-1, -2) 포함 — 의도된 설계 (반대 유형 억제용) |
| 전체 | AdSense pub ID는 `ca-pub-XXXXXXXXXXXXXXXX` 플레이스홀더 — 배포 전 실제 ID로 교체 필요 |

---

## 📋 index.html 준비 중 테스트 (향후 추가 예정)

| 제목 | 상태 |
|---|---|
| 나의 스트레스 유형 | 준비 중 |
| 나의 직업 유형은? | 준비 중 |
| 2026 나의 운세는? | 준비 중 |

---

## 📝 변경 이력

| 날짜 | 변경 내용 |
|---|---|
| 2026-03-08 | 초기 매니페스트 작성. love-style 20문항/8유형으로 확장. toggleLang 버그 수정. 중복 compat-card 제거. index.html 정보 업데이트(3분/8유형/20문항/32+/2026운세). |
| 2026-03-08 | hell-test.html 신규 추가 (15문항/6유형/KO+EN). index.html 테스트 수 4→5, 결과 유형 32+→38+로 업데이트. 기존 4개 테스트 더보기 섹션에 hell-test 링크 추가. |
