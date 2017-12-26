# js_optimization_handbook
javascript optimization handbook
자바스크립트 최적화 핸드북

## Array
- 일반적으로 임시 컨테이너로 사용하는 Array데이터.
- Array를 정리하는 가장 효율적인 방법은
```js
const array = [1, 2, 3, 4, 5]
array.length = 0
console.log(array) // []
```

## String 파싱

```js
const num = '10.9';
const numst = '10m';

parseInt(num)	// 10
parseInt(numst)	// 10

~~num // 10
~~numst // 0

+num // 10.9
+numst // NaN
```
소수점이 있는 숫자는 +num
정수(문자가뒤에 섞여 있는)는 parseInt


## 메모리

```js
const foo = { bar: 'hello world' }
delete foo.bar // Inefficient way (bad)

const foo = { bar: 'hello world' }
foo.bar = undefined // Efficient way (good)
```

## 조회 및 탐색

```js

```
