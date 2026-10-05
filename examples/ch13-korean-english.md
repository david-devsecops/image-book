# Chapter 13 한국어와 영어 비교

[예제 목록](README.md) · [책 본문](../pages/033-ch13.md)

## 실습 목표

첫 잔 프롬프트를 영어로 옮겼을 때 의미가 유지되는지 확인합니다.

아래 코드 블록의 내용만 복사해 이미지 생성 도구에 입력하세요. 편집 단계에서는 지정한 입력 파일을 먼저 첨부합니다.

비교할 [한국어 프롬프트와 원본 결과](ch04-first-image.md)를 먼저 확인하세요.

## 1. 영어 프롬프트

입력: 텍스트만 사용합니다. 첨부 이미지는 없습니다.

```text
Create a photograph of one cream-colored matte ceramic mug on a white table. The handle is on the right, and the entire mug is visible. The background is plain light gray with no pattern. Use soft light coming from a window on the left, with a natural shadow cast to the right. View it from slightly above eye level and place the mug in the center of a square frame. Do not include text, logos, people, or other props.
```

### 수록 결과

![영어 프롬프트 결과](../assets/mug-english.png)

AI 생성 이미지. Codex 내장 imagegen, 모델 ID 미공개, 2026-10-05. PNG 1254×1254, RGB. 생성 1회, 수록 1장.

[결과 파일 열기](../assets/mug-english.png)

### 결과 관찰

충족한 조건: 크림색 잔 하나, 오른쪽 손잡이, 흰 탁자, 회색 배경과 정사각형 구성이 나타났습니다.

달라진 점: 한국어 결과보다 몸체가 곧고 높아 보이며 손잡이 안쪽 구멍이 세로로 길어졌습니다. 벽과 탁자의 경계도 더 낮습니다.

판정: 기본 조건 충족, 한국어 결과와 개체 형태 차이 확인.

## 바꿔 볼 조건

짧은 한국어 요청을 번역한 뒤 대상, 수량, 배치가 추가되거나 빠지지 않았는지 대조하세요.

응용 과제는 위에 수록한 실제 실행 기록에 포함되지 않습니다.

[책의 설명과 검수 기준](../pages/033-ch13.md) · [예제 목록](README.md)
