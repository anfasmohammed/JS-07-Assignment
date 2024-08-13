1. 	Write short notes on below array methods with code examples
   •	reverse()
   •	sort()
   •	fill()
   •	filter()
   •	some()
   •	every()
   •	map()
   •	forEach()
   •	reduce()
   •	indexOf()

Ans.
- reverse() : This method in JavaScript is used to reverse the order of elements in an array.

- Eg :
```js 
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.reverse();
console.log(fruits);
```
- sort() : This method in JavaScript is used to sort the elements of an array in place and returns the sorted array. By default, it sorts the elements as strings in alphabetical and ascending order.

- Eg :
```js
let fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
console.log(fruits);
```
- fill() : This method in JavaScript is used to fill all the elements of an array from a start index to an end index with a static value.

- Eg :
```js
let arr = [1, 2, 3, 4, 5];
arr.fill(0, 1, 4);
console.log(arr);
```
- filter() : This method in JavaScript is used to create a new array with all elements that pass a test implemented by a provided function.

- Eg :
```js
let arr =[1,2,3,4,5]
let result=arr.filter((item)=>{
    return item%2==0
})
console.log(result);
```
- some() : This method in JavaScript is quite useful! It checks if at least one element in an array passes a test provided by a function.

- Eg :
```js
let arr=[6,2,1,4,10]
let isEven=(num)=>{
    return num%2===1
}
let output=arr.some(isEven)
console.log(output);
```
- every() : This method in JavaScript is used to test whether all elements in an array pass a specified test implemented by a provided function.

- Eg :
```js
let arr=[6,2,8,4,10]
let isEven=(num)=>{
    return num%2===0
}
let output=arr.every(isEven)
console.log(output);
```
- map() : This method in JavaScript is a powerful array method used to create a new array by applying a specified function to each element of the original array.

- Eg :
```js
let arr=[1,2,3,4,5]
arr.map((item)=>{
    console.log(item*2);
    
})
```
- forEach() : This method in JavaScript is used to execute a provided function once for each array element.

- Eg : 
```js 
let arr=[1,2,3,4,5]
let isEven=(num)=>{
    return num%2===0
}
arr.forEach((item)=>{
    console.log(isEven(item));
    
})
```
- rsduce() : This method in JavaScript is a powerful tool for array manipulation. It executes a reducer function on each element of the array, resulting in a single output value.

- Eg :
```js
let arr=[100,10,20]
let myFunction=(accumulator,currentValue)=>{
    return accumulator-currentValue
}
let result=arr.reduce(myFunction)
console.log(result);
```
- indexOf() : This method is used to find the position of a specified value within a string or an array.If the value is not found, it returns -1.

- Eg :
```js
let animals=["ant","bison","camel","bison"]
console.log(animals.indexOf("camel"));
console.log(animals.indexOf("bison"));
console.log(animals.indexOf("elephant"));
```

2.	write a function that takes an array of numbers as an argument and returns the sum of its elements.

Ans.
```js
let arr=[100,10,20]
let myFunction=(accumulator,currentValue)=>{
    return accumulator+currentValue
}
let result=arr.reduce(myFunction)
console.log(result);
```

3.	Create a function that filters strings in an array by their length

Ans.
```js
let animals=["ant","bison","camel","bison"]
let filtered=animals.filter((item)=>item.length>3)
console.log(filtered);
```

4.	Create a function that returns a new array containing the square roots of each number in the original array [1,4,9,16,25]
(Math.sqrt())

Ans.
```js
let numbers=[1,4,9,16,25]
numbers.forEach((item)=>console.log(Math.sqrt(item)))
```

5.	Write a function that prints the number 1 to 100. But for multiples of 3, print Fizz instead of the number, and for multiples of 5, print Buzz. For the numbers that are multiples of both 3 and 5, print FizzBuzz.

Ans.
```js
let printNumber=(endValue)=>{
    for (let num=1;num<=endValue;num++){
    if (num%3==0&num%5==0){
    console.log("FizzBuzz");
    
    }
    else if(num%5==0)
    {console.log("Buzz");
    }
    else if(num%3==0)
    {
        console.log("fizz");
        
    }
    else {
        console.log(`${num}`);
        
    }}}
printNumber(100)
```











