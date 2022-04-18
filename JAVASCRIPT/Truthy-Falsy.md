# Truthy & Falsy
참과 같은 값 / 거짓과 같은
값
<br>
<br>

## Truthy
사실상 무한대에 가깝기 때문에 Falsy값을 기억하는 것이 빠르다
<br>
<br>

## Falsy
```js
if (false)
if (null)
if (undefined)
if (0)
if (-0)
if (NaN)
if (0n)
if ('')

if (' ') // 공백 문자는 Truthy이다
```
부정적인 느낌은 Falsy

**주의할 것은**, 공백 문자가 들어 있는 경우, **Truthy**이다