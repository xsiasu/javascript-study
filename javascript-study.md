# ECMA SCRIPT 6
## let 변수사용하기

```javascript
var snack ="saeukang"
function getFood(food) {
    if(food){
        var snack = "potato"
        return snack
    }
    return snack
}


console.log(getFood(false))   

//undefind     function getFood(food).. 가 false이므로 해당함수를 건너뛰고 전역변수를 가져올것으로
//예상하지만 undefind 가 실행된다. "{"스콥은 
```
## ECMA SCRIPT 6에서 let변수 사용하는 법
### let은 block scop 
```javascript
let snack ="saeukang"
function getFood(food) {
    if(food){
        let snack = "potato"
        return snack
    }
    return snack
}

console.log(getFood(false));
// saeukang 출력
console.log(getFood(true));
// potato 출력 
```

## 화살표 함수
```javascript
function Person(name) {
    this.firstName = name;
}

Person.prototype.prefixName = function(arry){
    return arry.map((charactor,index) => {
        return index + charactor +''+ this.firstName
    })
}

const person = new Person('SEAN')
console.log(person)
console.log(person.prefixName(['kim','lee']))


const object = {
    name : 'this object',
    func : function(){
        console.log(this)
    }
}

object.func()
```
##
```javascript
function SomeObject(name) {
    this.name = name;
    console.log(this)
}
```
```javascript
const object = {
    name : 'object nameddd',
    func : () => {
    console.log(this)
    }
}

object.func()
```
