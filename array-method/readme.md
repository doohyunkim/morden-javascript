array method ( filter ,map, reduce )
-

```
const fruits = [	"apple", "pear", "peach" ]

console.log( fruits.join(", ") )
// "apple, pear, peach"

console.log( fruits.filter( fruit=>fruit[0] ==="p") )
// ["pear", "peach]
	
console.log( fruits.map( fruit=> `big ${fruit}`) )
// ["big apple", "big pear", "big peach"]

console.log ( fruits.map( fruit=> ({ name: fruit}) ) )


```
