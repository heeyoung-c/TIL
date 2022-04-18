# Type-Conversion(형변환)

```js
const a = 123
const b = 123

console.log(a == b)
// 동등 연산자

const c = 123
const d ='123'

console.log(c == b)
// true
```
형변환

자동으로 값이 변환되어 true 값으로 나옴

동등 연산자는 쓰지 말 것!

```js
const a = 1
const b = true

console.log(a == b)
// true
```
이러한 문제 때문에

일치 연산자를 사용한다

```js
const a = 1
const b = true

console.log(a === b)
// false
```

`===` 완전히 같은 지 확인 하는 것

일치 연산자는 메모리 주소를 비교한다

```js
const a = 1
const b = 1
console.log(a === b)
//true

const a = []
const b = []
// true가 나올 수도 있고, false가 나올 수도 있다.
// 어떤 메모리 주소를 바라보는지를 알아야 한다
```

원시형은 생긴 게 같으면 주소가 같다

참조형은 생긴 게 같아도 주소가 다를 수 있다