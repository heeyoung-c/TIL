# CSS-Conding-Convention

## Mozilla
> 모질라에서 제안한 CSS속성 기술 순서

1. `display`
2. `list-style`
> 객체의 노출 여부와 표현방식
--- 
3. `position`
4. `float`
5. `clear`
> 위치와 좌표
---
6. `width` / `height`
7. `padding` / `margin`
> 크기와 여백
---
8. `border` / `background`
> 윤곽과 배경
---
9. `color` / `font`
10. `text-decoration`
11. `text-align` / `vertical-align`
12. `white-space`
> 글자와 정렬
---
13. other text
14. content
> 내용
---
<br>
<br>

## Naver
> 
1. `display` (표시)
2. `overflow` (넘침)
> 객체의 노출 여부와 표현 방식
---
3. `float` (흐름)
4. `position` (위치)
> 위치
---
5. `width` / `height` (크기)
6. `padding` / `margin`(간격)
7. `border`(테두리)
8. `background`(배경)
> 윤곽과 배경
---
9. `color` / `font`(글꼴)
10. `animation`
---
<br>
<br>

## 결론은..

###
1. `display`
2. `overflow`
3. `line-style`
> 화면 표시 방법 > 출력의 범위 > 표시된 내용의 테두리 표현
---
4. `position`
5. `float`
6. `clear`
> 표시할 위치
---
7. `width` / `height`
8. `padding` / `margin`
9. `border` / `background`
> 가로 세로 값 > 간격 > 테두리 > 배경
---
10. `color` / `font`
11. `text-decoration`
12. `text-align` / `vertical-align`
13. `white-space`
> 글자 색상, 종류 > 정렬 > 글자 처리 방법
---
14. `animation`