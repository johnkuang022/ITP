# FizzBuzz

To start the assignment, I copied the "for loop" code that generated all the numbers between 1 and 100.

```for (let x = 1; x < 100; x++) ```

My next steps were to set up the parameters that would make the console print out the texts to the corresponding numbers. 

I used Modulo to find the numbers divisible by 3 and by 5, and then numbers that are divisible by both of those numbers. I then assigned "Fizz," "Buzz," and "Fizzbuzz" to them.

I then realized that when the console prints the results, the numbers divisible by both numbers will print out three results:

``Fizz
Buzz
Fizzbuzz``

I then fixed this issue by adding extra parameters to the "if" statements detecting for numbers divisible by 3 and by 5, by using another "&&" to make sure they don't print when the number is divisible by both 3 and 5. 

``if (x % 3 === 0 && x % 5 > 0) {
    console.log("Fizz")
  }
  if (x % 5 === 0 && x % 3 > 0) {
    console.log("Buzz")
  }
``
  
  Then I ran the code, and it worked perfectly.
  
```

for (let x = 1; x < 100; x++) {
  if (x % 3 === 0 && x % 5 > 0) {
    console.log("Fizz")
  }
  if (x % 5 === 0 && x % 3 > 0) {
    console.log("Buzz")
  }
  if (x % 5 === 0 && x % 3 === 0) {
    console.log("FizzBuzz")
  }
  if (x % 5 > 0 && x % 3 > 0){
    console.log(x)
  }

}

```


###I learned that moving up an "if" statement gives it priority over the code that is below it.