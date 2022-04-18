# Variable(변수)

```js
const a = 123
// a 라는 변수에 123이라는 숫자 데이터를 담는다
```
만약 메모리의 주소를 '서울' 이라고 해보자

a라는 변수는 '서울' 메모리 주소를 바라보고 있다

`console.log(a)`를 하는 경우, '서울' 메모리에서 숫자 데이터 `123`을 가져오는 것이다
<br>
<br>

## 변수 선언의 차이점

- 유효범위(Scope)
- 재할당 가능 여부
- 중복 선언 가능 여부
- 호이스팅(Hoisting)
- 전역(Global) 선언시 전역 객체(`window`)의 속성으로 등록


1. `const`
    - 유효범위: 블록 레벨
    - 재할당: X
    - 중복 선언: X
    - 호이스팅(Hoisting): X
    - 전역 등록: X

2. `let`
    - 유효범위: 블록 레벨
    - 재할당: O
    - 중복 선언: X
    - 호이스팅(Hoisting): X
    - 전역 등록: X

3. `var`
    - 유효범위: 함수 레벨
    - 재할당: O
    - 중복 선언: O
    - 호이스팅(Hoisting): O
    - 전역 등록: O

>이제 `var`는 사용하지 않는 추세이다

```js
// var
function abc() {
  if (true) {
    var a = 123
    console.log('in', a)
  }
  console.log('out', a)
}
abc ()
// in 123
// out 123


// let
function abc() {
  if (true) {
    let a = 123
    console.log('in', a)
  }
  console.log('out', a)
}
abc ()
// in 123
// a is not defined


// const
function abc() {
  if (true) {
    const a = 123
    console.log('in', a)
  }
  console.log('out', a)
}
abc ()
// in 123
// a is not defined
```
`var`는 함수 레벨 범위 에서는 유효하다

`let, const`는 블록 레벌 범위 에서 유효하다
<br>
<br>

## 재할당
`const`(constant)(상수)

의미적으로는 상수라고 부르지만, 정확하게는 변수이다

상수라는 개념은 값을 다시 할당할 수 없기 때문에 재할당 할 수 없다

```js
const a = 123
a = 456
// X 재할당 불가능
```
<br>
<br>

## 중복 선언
```js
const a = 123
const a = [5, 6, 7]
// XX
```
<br>
<br>

## 호이스팅

코드는 위에서 부터 아래로 평가된다

간단하게 설명하자면

선언은 밑에서 되고, 사용은 위에서 하는 경우

밑에 있는 선언부를 위로 끌어 올려서 사용하는 것

선언부가 유효범위의 최상단으로 끌어 올려지는 현상

```js
console.log(a) // X
console.log(b) // undefined

const a = 1234
var b = 5678
```
`var`의 경우 `undefined`라는 값이 할당되어 있는 것이다
<br>
<br>

## 전역 범위

```js
var heeyoung = 123

console.log(window.heeyoung)
// 123
```
사이트가 뜨고있는 창에 대한 정보는 `window`에 다 들어와있는데,

`window.heeyoung` 는 `123` 이 나온다
<br>
<br>

## 결론 ...

일단 `const`를 쓴다

재할당이 필요한 경우에만 `let`을 쓴다