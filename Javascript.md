## Javascript

### Destructuring

[[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment|Destructuring]]
is where you can unpack values from arrays, or properties from objects, and
then place them into variables

Example of Assigning variables from a nested object
Create variables lowToday and highToday from the values of today.low and
today.high
`const LOCAL_FORECAST = { yesterday: { low: 61, high: 75 }, today: { low: 64, high: 77 }, tomorrow: { low: 68, high: 80 } }; const {today: {low: lowToday, high: highToday}} == LOCAL_FORCAST;`
