# 부록 D 표지 제작 프롬프트

[예제 목록](README.md) · [책 본문](../pages/093-records.md)

## 실습 목표

제목의 가독성과 표지 비율을 함께 요청한 실제 예를 살펴봅니다.

아래 코드 블록의 내용만 복사해 이미지 생성 도구에 입력하세요. 편집 단계에서는 지정한 입력 파일을 먼저 첨부합니다.

표지의 영어 프롬프트 선택 이유는 책 본문의 저자 확인 항목으로 남아 있습니다.

## 1. 표지 생성

입력: 텍스트만 사용합니다. 첨부 이미지는 없습니다.

```text
Create a polished Korean technical nonfiction book cover as a FLAT RECTANGULAR PNG, exact portrait aspect ratio 100:130 (width:height), ideally 1600x2080. NOT a 3D book mockup. Title in very large, crisp, perfectly spelled Korean on upper two thirds: '처음 시작하는' then 'AI 이미지' then '프롬프트'. Small subtitle: '원하는 그림을 말로 설명하는 방법'. A sophisticated contemporary editorial design, warm ivory background, near-black Korean typography, cobalt blue and terracotta restrained accents. Bottom third shows a beautiful still life: simple cream ceramic mug, one small green leaf, and abstract framing lines suggesting composition and image creation. No company logos, no author name, no dates, no extra words, no watermarks. Spacious margins, very readable at thumbnail size. Text must be the dominant design element. This is an independently created cover for a beginner textbook.
```

### 수록 결과

![표지 생성 결과](../assets/cover.png)

AI 생성 이미지. Codex 내장 imagegen, 모델 ID 미공개, 2026-10-05. PNG 1100×1430, RGB. 생성 1회, 수록 1장.

[결과 파일 열기](../assets/cover.png)

### 결과 관찰

희망 크기는 1600×2080으로 요청했지만 실제 결과는 1100×1430입니다. 비율은 요청과 일치합니다. 이 차이를 숨기지 않고 실제 파일 수치를 기록했습니다. 표지는 첫 페이지와 같은 파일을 사용합니다.

## 바꿔 볼 조건

자신의 제목으로 바꾸기 전에 정확한 문구, 줄바꿈과 제목의 크기 순서를 먼저 정하세요.

응용 과제는 위에 수록한 실제 실행 기록에 포함되지 않습니다.

[책의 설명과 검수 기준](../pages/093-records.md) · [예제 목록](README.md)
