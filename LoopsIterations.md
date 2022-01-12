# Loops and Iteration

## Level 1

---

Write a function in Javascript to print the following pattern.



let n=5;
let str = "";

for(let i=1; i<=n; i++) {
for(let j=1; j<=n-i; j++) {
str += "";
}
for(let k=1; k<=2*i-1; k++) {
str += k;
}
str +="\n"
}
```
      1
    1 2 1
  1 2 3 2 1
1 2 3 4 3 2 1
```

The function can take the number of rows as input. The pattern should be printed in the console. Minimum number of rows should be 3.

## Level 2

---

Write a function in Javascript to print the sum of the first n fibonacci numbers.



function SumofFibbonacci(n) {

let fib = [];
if(n<=0) {
return 0
}

fib[0]=0;
fib[1] = 1;

let sum = fib[0] + fib[1];

for(let i=2; i<=n; i++) {
fib[i] = fib[i-1] + fib[i-2];
sum += fib[i];
}

return sum;
}

**Input:** 6

**Output:**

```
1 1 2 3 5 8
Sum: 20
```

## Level 3

---

Normalize the following object to an array of objects.

const newObj = [];

Object.keys(obj).forEach(key => newObj.push({
...obj[key],reaction: key
}))

