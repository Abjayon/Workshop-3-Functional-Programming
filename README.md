# Workshop-RXKS
An InDepth Introduction to RXJS

#### Legends   
📝 - Article  
🧠 - Important ( Must To Know )  
🚀 - Hard  
🍕 - Easy  
🐱‍👤 - New Skill  



### 📚Resource to Learn and Go through :  

# Functional Programming 101

Hi All, before we jump into learning about functional programming,  want to create a **RoadMap** which is needed to get a good grasp on Functional Programming.

### Functional Patterns

So if you have pure funtions you can apply simple math rules on them.
```js
// associative
add(add(1,2),3) == add(1, add(2,3))

// commutative
add(4,1) = add(1,4)

// identity 
add(n,0) == n


//distributive
multiply(2, add(3,4)) == add(multiply(2,3), multiply(3,4))
```

> Polymorphic Composable Interfaces

### Arity
The number of arguements a functions takes. Comes from a word like unary, binary, ternary etc.

```js
// Unary Function
const greet = (name) => `Hi ${name}`;

// Binary Function
const add => (a, b) => a + b;
```

Functions where the number of arguements is not defined are called "Variadic" functions.

### High Order Functions
A function which takes a function as arguement and/or returns a function.

```js
const double = x => x*2;

const doubleArray = [1, 2, 3].map(double);
```

### Closure
A closure is a property which lets you access a variable outside it's scope. Formally, a closure is a technique for implementing lexically scopend named bindings. It is a way of storing a function within an environment.
```js
const add = (x) => (y) => x + y;
const addTen = add(10);
const addFive = add(5);

addTen(43) // 53
addFive(43) // 48
```
- [ ] [What is a closure](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36) 
#### Further Reading
- [Lamda vs Closure](http://stackoverflow.com/questions/220658/what-is-the-difference-between-a-closure-and-a-lambda)
- [Understand Closure Working](http://stackoverflow.com/questions/111102/how-do-javascript-closures-work)

### Partial Application
Partial Application is the process of creating functions via calling an original function with fewer arguements. The function returned by original function will ask for remaining arguements.

You can also think of partial application by splitting of invocation of functions in small steps.


### Currying
The process of converting a function that takes multiple arguments into a function which take one at a time.
Each time you call this function you pass one arguement. It will return you another function which will ask for another arguement.

```js
const finalPriceCurried = (discount) => (price) =>  price - ((discount/100) * price); 

const nonPrimeMemberPrice = finalPriceCurried(40);
const primeMemberPrice = finalPriceCurried(50);

nonPrimeMemberPrice(500) // 300
primeMemberPrice(500) //
```

## Functional Terminology 

### Purity

### Side Effects

### Idempotent

### Point Free Style

### Dot Chaining


## Resources 
Firstly get familiar with all new JS syntax (**ES5, ES6, ES7**).
You should learn all the described syntax by heart.
- [ ] [JS Features](https://jsfeatures.in/)

You will be able to easiy follow this if you are comfortable with Functional Array Methods (Map and Reduce)
- [ ] [Gentle Introduction To Functional Programming](https://jrsinclair.com/articles/2016/gentle-introduction-to-functional-javascript-intro/)

Consider this as Bible of Functional Programming in JS.
- [ ] [Mostly Adequate Guide To Functional Programming](https://mostly-adequate.gitbooks.io/mostly-adequate-guide/)


### Inspiration Resources
These are some articles explaining people who get started with Functional Programming :
- [ ] [How I get Started with functional Programming](https://dev-self-start.blogspot.com/)


