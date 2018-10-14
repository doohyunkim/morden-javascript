arrow function
-
traditional function<br>
```
var road = function(detail){
	return `korea, seoul, guro ${detail}`
}
console.log( road("saemalo")) //korea,seoul,goru
```
arrow function
```
var road = detail => `korea, seoul, guro ${detail}`

var road2 = (detail1,detail2) => `${detail1} is ${detail2}`
```


warning : arrow function은 새롭게 this를 생성하지 않음<br>
즉, this를 사용하여 영역 유지를 할 수 있음.
<br><br>
arrow funciton : binding 영역이 유지됨 <br>
traditional function : new this binging
```
var coin = {
	kinds: [ "10","50","100","500"],
	print: function(delay=100){
		setTimeout(() => {
			console.log(this.kinds.join(","))
		}, delay)
	}
}
```
