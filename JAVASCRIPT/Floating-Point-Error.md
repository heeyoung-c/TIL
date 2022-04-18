# Floating-Point-Error
>컴퓨터가 숫자를 표시하는 방법에 한계가 있기 때문에, 십진수를 이진수로 변환하는 과정에서 발생하는 오류

```js
const a = 0.1
const b = 0.2
console.log(a + b) 
// 0.30000000000000004

const a = 0.1
const b = 0.2
console.log(
  (a + b).toFixed(1)
// 0.3
// 하지만 이런 경우에 문자가 출력된다

const a = 0.1
const b = 0.2
console.log(
  parseFloat((a + b).toFixed(1))
)
//정상적으로 숫자가 출력된다
```
## 결론 ...
`toFixed( )`를 사용하면 문자가 출력되기 때문에<br>
`parseFloat`를 사용하면 정상적으로 숫자를 출력 할 수 있다