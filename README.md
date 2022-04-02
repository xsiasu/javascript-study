# ECMA SCRIPT 6
## const, let 변수사용하기


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
예상하지만 undefind 가 실행된다. "{"스콥은 


let snack ="saeukang"
function getFood(food) {
    if(food){
        let snack = "potato"
        return snack
    }
    return snack
}

console.log(getFood(false));
