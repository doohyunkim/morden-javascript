
var, let, const 
-
기능<br>
var > let > const<br>
```
var = redeclare, change value.<br>
let = **not** redeclare, change value. <br>
const = **not** redeclare, **not** change
```
Scope<br>
var = function scope <br>
let, const = block-scope <br>

```
var topic = "javascript"
if(topic) {
	let topic = "react"
	console.log('block', topic) //(global react)
}
console.log('global', topic) // (global javascript)
// if it's declare var, console.log print global react twice
```