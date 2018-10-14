object & array (ES6)
-

구조분해 (destructuring) <br>
일종의 변수 할당 취급

```
var hamburger = {
 bread : "참깨빵",
 meat: "소고기",
 toppings: ["양파","치즈","양상추"]
}

var {bread,meat} = hamburger
console.log(bread, meat) // 참꺠빵 소고기
```

객체 또한 넘길 수 있음

```
var road = address =>{
	console.log(`Korea, ${address.city}`)
}

var address ={
	city: "seoul",
	gu: "guro"
}
road(address)
```

스프레드 연산자<br>
1. array merge

```
var a = ["1","2","3"]
var b = ["4","5"]
var c = [...a, ...b]	//c = [1,2,3,4,5]

```

2. copy array
(원본 보존)

```
var a = ["1","2","3"]
var [last] = [...a].reverse()	//a는 원형 유지 (reverse는 원래 원형을 변경하는 함수)
console.log(last) // 3
```

3. 일부 가져오기

```
var a=["1","2","3","4","5"]
var [first, ...rest] = a
console.log(rest)	//2,3,4,5
```
