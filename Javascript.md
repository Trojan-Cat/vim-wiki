## Javascript

### Destructuring

[[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment|Destructuring]]
is where you can unpack values from arrays, or properties from objects, and
then place them into variables

Example of Assigning variables from a nested object
Create variables lowToday and highToday from the values of today.low and
today.high

````
const LOCAL_FORECAST ={
  yesterday: { low: 61, high: 75 },
  today: { low: 64, high: 77 },
  tomorrow: { low: 68, high: 80 }
};

const {today: {low: lowToday,high: highToday}} == LOCAL_FORCAST;```
````

### Looping

[[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration|Loops]]
A loop is a quick way to do something repeatedly

#### Continue

If you're checking for a type in a loop, and it comes up but you want to skip
it and keep the loop going you use a continue

- First check for the type or argument
- Then add continue at the end if that's what you want to skip in a loop
  `if(typeof arr[i] !== 'string') continue`
  This will check the arr[i] variable to see what type it is, if it's not
  a string type, it'll skip it

#### Break

This is similar to the continue except that rather than skipping it stops the
loop there if that condition is found.
