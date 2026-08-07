# 애들아 다들 이거 합쳐봐 ㅈㄴ세짐

생년월일 입력 → **음력 기준 정확한 띠** + 별자리 합체 이름 생성기

> 전갈자리 + 토끼띠 = **전갈토끼**

[Live Demo](https://zodiac.allsweep.xyz/)

## Features

- 음력(설날) 기준 정확한 띠 계산
- 12 별자리 × 12 띠 = **144개 조합** 전부 지원
- 조합마다 결정적(해시)으로 다른 설명 + 브랜딩 문구
- Bright Brutalism UI (두꺼운 테두리 + 하드 그림자 + 형광 포인트)
- 순수 정적 사이트 (백엔드 없음)

## Tech

- HTML / CSS / Vanilla JS
- [lunar-javascript](https://github.com/6tail/lunar-javascript) (CDN) — 음력·생肖 계산
- Black Han Sans + Space Mono

## How it works

1. 생년월일 입력
2. `Solar.fromYmd()` → 음력 띠 추출
3. 월·일로 서양 별자리 판별
4. `별자리이름 + 띠` 합체 이름 생성
5. 조합 문자열을 해시해서 설명/브랜딩 템플릿 선택 (같은 조합 = 항상 같은 결과)

## Structure

```
index.html   # 단일 파일 (스타일 + 로직 전부 포함)
CNAME        # zodiac.allsweep.xyz
```

## License

MIT
