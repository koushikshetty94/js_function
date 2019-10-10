1. 🎖Write a function named calculateDogAge that:
  * [ ] Takes 1 argument: your puppy's age.
  * [ ] Calculates your dog's age based on the conversion rate of 1 human year to 7 dog years.
  * [ ] Outputs the result to the screen like so: "Your doggie is NN years old in dog years!"
  * [ ] Add an additional argument to the function that takes the conversion rate of human to dog years.

```js
// your code goes here
 let age1 =+prompt("enter puppyage");
        let age2 =+prompt("enter conversion rate");
        function calculateDogAge(humanYears = 1,puppyAge = 7){
            var dogAge;
            dogAge = puppyAge * humanYears;
            document.write(`${dogAge}`);
        }
        calculateDogAge(age1,age2);
```
2. 🎖Write a function named calculateSupply that:
  * [ ] takes 2 arguments: age, amount per day.
  * [ ] calculates the amount consumed for rest of the life (based on a constant max age).
  * [ ] outputs the result to the screen like so: "You will need NN to last you until the ripe old age of X"
  * [ ] Accept floating point values for amount per day, and round the result to a round number.

```js
// your code goes here
 const maxAge=85;
        function calculateSupply(){
            let age=+prompt(" enter age");
            let amtPerDay=+prompt(" enter amount per day ");
            let amountReqd=(( maxAge - age ) * 365) * amtPerDay;
            alert(`you will need ${amountReqd} to last you until the ripe old age of ${age}`);
        }
        calculateSupply();
```
3. 🎖Create a function called celsiusToFahrenheit:
  * [ ] Store a celsius temperature into a variable.
  * [ ] Convert it to fahrenheit and output "NN°C is NN°F".
  * [ ] Create a function called fahrenheitToCelsius:
  * [ ] Now store a fahrenheit temperature into a variable.
  * [ ] Convert it to celsius and output "NN°F is NN°C."

```js
 let celciusTemp = 0;
        celciusTemp = +prompt("enter the degree is celcius");
        let farenheitDegree;
        function celciusToFarenheit(){
            farenheitDegree=(celciusTemp*(9/5) + 32);
            alert(`${celciusTemp}C is ${farenheitDegree}C`);
        } 
        celciusToFarenheit();
        let farenheitTemp=+prompt("enter the degree in farenheit");
        let celciusDegree;
        function farenheitToCelcius(){
            celciusDegree = (farenheitTemp-32)*1.8;
            alert(`${farenheitTemp} C is ${celciusDegree} C`)
        }
        farenheitToCelcius();
// your code goes here
```
4. 🎖The function below returns true if the parameter age is greater than 18. Otherwise it asks for a confirmation and returns its result:

```js
function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    // ...
    return confirm("Did parents allow you?");
  }
}
```
  4.1 🎖Convert the above function using ternary operator.
  ```js
    function checkAge(age) {
    return (age > 18)? true : confirm("Did parents allow you?");
    }
  // your code goes here
  ```

  4.2 🎖Convert the above function using `||` operator.
  ```js
    function checkAge(age) {
    return (age > 18) ||  confirm("Did parents allow you?");
    }
  // your code goes here
  ```
Will the function work differently if else is removed like below?

```js
function checkAge(age) {
  if (age > 18) {
    return true;
  }
  // ...
  return confirm("Did parents allow you?");
}
```
Is there any difference in the behavior of these two variants? If there is what is that?


5. 🎖 Write a function pow(x,n) that returns x in power n.

  * [ ] Use prompt to take values for x and n, and then shows the result of pow(x,n) using alert.
  * [ ] In this task the function should support only natural values of n: integers greater then 1.

```js
// Your code goes here

let x=+prompt("enter base");
        let n=+prompt("enter exponential");
        let sum;
        function pow(x,n){
            sum=x**n;
            alert(sum);
        }
        pow(x,n);

// After writing code uncomment to check the answer.
// pow(3, 2); // 9
// pow(3, 3); // 27
// pow(1, 100); // 1
// pow(-31, 2); // "The number below 1 is not allowed"

6. 🎖Write a program that asks the user for a number n and gives them the possibility to choose between computing the sum and computing the product of 1,…,n. Return the result accordingly.

```js
// your code goes here
```
6. 🎖Write a program that asks the user for a number n using prompt and prints the sum of the numbers 1 to n

```js
function numberSum() 
        {
            let n = +prompt("enter");  
            var sum=0;
            for(var i=1; i<=n; i++){
            sum += i; 
            }
            return sum;
        }
        numberSum();

// your code goes here
```
7. 🎖Modify the previous program such that only multiples of 5 or 7 are considered in the sum, e.g. n = 20 (5,7,10,14,15,20) 71

```js
 function numberSum() 
        {
            let n = +prompt("enter");  
            var sum=0;
            for(var i=1; i<=n; i++){
                if(i % 5 == 0 || i % 7 == 0){
                    sum += i; 
                }
         
            }
            return sum;
        }
        numberSum();
// your code goes here
```

8. 🎖Write a function `min` that takes two arguments and returns their minimum.

```js
// Your code here.

console.log(min(0, 10));
// → 0
console.log(min(0, -10));
// → -10
```
let num1 = +prompt("enter num1");
        let num2 = +prompt("enter num2");
        function min(num1,num2){
            if(num1>num2){
                alert(`${num2} is smaller than ${num1}`);
            }
            else if (num2>num1){
                alert(`${num1} is smaller than ${num2}`);
            }
        }
        min(num1,num2);
