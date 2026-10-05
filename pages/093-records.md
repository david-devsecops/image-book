## 실행한 범위

모든 생성·편집은 2026-10-05에 Codex 내장 imagegen으로 수행했습니다. 최초 7회에 이번 개정의 14회를 더해 총 21회 실행했고, 결과 21장을 모두 수록했습니다. 정확한 이미지 모델 ID, 시드, 내부 품질 파라미터는 도구 응답에서 확인되지 않았습니다. 외부 사진이나 수집 이미지는 입력하지 않았습니다.

한 번의 실행 결과를 도구 전체의 성능으로 일반화하지 않습니다. 자연어로 지정한 배치·색·유지 조건은 목표를 설명하며, 정확한 좌표나 픽셀 보존을 보장하는 명령은 아닙니다. 따라서 이 책에서는 요청한 조건과 실제 파일·화면을 따로 확인합니다.

아래 표의 ‘1회’는 파일별 생성 또는 편집 호출 한 번을 뜻합니다. 동일 이미지를 여러 장에서 인용해도 수록 파일 수에는 한 번만 셉니다. 판정은 해당 장의 육안 관찰이며 파일 속성은 저장 파일에서 측정했습니다.

| 결과 파일 | 입력과 작업 | 실행 / 수록 | 실제 속성 | 판정과 관찰 |
| --- | --- | --- | --- | --- |
| `cover.png` | 텍스트에서 표지 생성 | 1회 / 1장 | PNG 1100×1430 RGB | 10:13 비율, 제목 육안 확인 |
| `mug-original.png` | 텍스트에서 잔 생성 | 1회 / 1장 | PNG 1254×1254 RGB | 잔 하나, 오른쪽 손잡이 |
| `mug-blue.png` | 잔 원본의 배경 편집 | 1회 / 1장 | PNG 1254×1254 RGB | 파란 벽, 잔·탁자 대체로 유지 |
| `reading-illustration.png` | 텍스트에서 삽화 생성 | 1회 / 1장 | PNG 1254×1254 RGB | 책과 새싹, 단순한 색 구성 |
| `reading-transparent.png` | 삽화 배경 제거 | 1회 / 1장 | PNG 1254×1254 RGBA | 알파 0~255, 형태·크기 변화 |
| `cafe-base.png` | 텍스트에서 메뉴 배경 생성 | 1회 / 1장 | PNG 1122×1402 RGB | 상단 여백, 잔과 배 두 조각 |
| `cafe-poster.png` | 메뉴 배경에 글자 추가 | 1회 / 1장 | PNG 1122×1402 RGB | 지정 문구와 가상 가격 확인 |
| `mug-light-soft.png` | mug-original.png, Ch08 | 1회 / 1장 | PNG 1254×1254 RGB | 유지 조건 충족, 조명 변화는 육안으로 작게 관찰됨 |
| `mug-light-hard.png` | mug-original.png, Ch08 | 1회 / 1장 | PNG 1254×1254 RGB | 직사광 표현 성공, 장면 전체의 명암 변화 동반 |
| `box-matte-paper.png` | 텍스트, Ch09 | 1회 / 1장 | PNG 1254×1254 RGB | 무광 종이 표현과 기본 구성 충족 |
| `box-metal.png` | 텍스트, Ch09 | 1회 / 1장 | PNG 1254×1254 RGB | 금속 표현 성공, 두 결과의 구도·색 일치 부분 실패 |
| `mug-green.png` | mug-original.png, Ch16 | 1회 / 1장 | PNG 1254×1254 RGB | 배경색 변경 성공, 주요 외형 육안 보존 |
| `mug-english.png` | 텍스트, Ch13 | 1회 / 1장 | PNG 1254×1254 RGB | 기본 조건 충족, 한국어 결과와 개체 형태 차이 확인 |
| `desk-base.png` | 텍스트, Ch17 | 1회 / 1장 | PNG 1254×1254 RGB | 제거 연습용 배치 충족 |
| `desk-eraser-removed.png` | desk-base.png, Ch17 | 1회 / 1장 | PNG 1254×1254 RGB | 지정 지우개·그림자 제거 성공, 주요 물체 육안 보존 |
| `mug-shelf.png` | mug-original.png, Ch19 | 1회 / 1장 | PNG 1254×1254 RGB | 장면 변경 성공, 개체 일관성 부분 충족 |
| `box-green-32.png` | 텍스트, Ch21 | 1회 / 1장 | PNG 1536×1024 RGB | 제품 시안의 기본 조건 충족, 문구 배치 전 그림자 확인 필요 |
| `box-blue-32.png` | box-green-32.png, Ch21 | 1회 / 1장 | PNG 1536×1024 RGB | 색 변경 성공, 주요 형태·배치 육안 보존 |
| `event-bg.png` | 텍스트, Ch23 | 1회 / 1장 | PNG 1024×1536 RGB | 안내 배경 조건 충족, 실제 행사 문구 배치는 미실행 |
| `story-01.png` | 텍스트, Ch24 | 1회 / 1장 | PNG 1254×1254 RGB | 장면 1의 대상·수량 충족 |
| `story-02.png` | 텍스트, Ch24 | 1회 / 1장 | PNG 1254×1254 RGB | 상태 변화 성공, 화분·소품·배경 일관성 부분 실패 |

실제 프롬프트는 표에 연결된 실습 장에 있습니다. 보존 실패와 조건 불일치도 그대로 수록했습니다. 특히 투명 배경 삽화의 형태 변화, 금속 상자의 구도 차이, 창가 잔과 스토리보드의 일관성 문제를 관찰 항목과 함께 확인하세요.

## 표지 제작 요청

<!-- TODO(저자): 표지 프롬프트를 영어로 작성한 이유 확인 -->

```text
Create a polished Korean technical nonfiction book cover as a FLAT RECTANGULAR PNG, exact portrait aspect ratio 100:130 (width:height), ideally 1600x2080. NOT a 3D book mockup. Title in very large, crisp, perfectly spelled Korean on upper two thirds: '처음 시작하는' then 'AI 이미지' then '프롬프트'. Small subtitle: '원하는 그림을 말로 설명하는 방법'. A sophisticated contemporary editorial design, warm ivory background, near-black Korean typography, cobalt blue and terracotta restrained accents. Bottom third shows a beautiful still life: simple cream ceramic mug, one small green leaf, and abstract framing lines suggesting composition and image creation. No company logos, no author name, no dates, no extra words, no watermarks. Spacious margins, very readable at thumbnail size. Text must be the dominant design element. This is an independently created cover for a beginner textbook.
```

희망 크기는 1600×2080으로 요청했지만 실제 결과는 1100×1430입니다. 비율은 요청과 일치합니다. 이 차이를 숨기지 않고 실제 파일 수치를 기록했습니다. 표지는 첫 페이지와 같은 파일을 사용합니다.

## 실행하지 않은 범위

본문의 ‘독자 과제’와 ‘독자 응용’은 학습자가 이어서 실행할 연습입니다. 스토리보드 장면 3·4, 행사 문구의 실제 배치, SNS 파생 이미지, API 호출, 실제 상품 촬영과 인쇄는 실행하지 않았습니다. WikiDocs 업로드와 전자책 변환도 로컬 제작 범위 밖에 있습니다.

`layout.png`, `workflow-eight.png`, `review.png`는 직접 구성한 교육용 도식 세 장입니다. 생성 이미지 21장의 실행 횟수에는 포함하지 않습니다. 작업 흐름 도식은 본문의 여덟 단계와 같은 순서로 수정했습니다. 이전 여섯 단계 도식은 개정 전 자료에 보존했습니다.

[이전 페이지](092-sources.md) · [전체 목차](../TOC.md) · [다음 페이지](094-publishing.md)
