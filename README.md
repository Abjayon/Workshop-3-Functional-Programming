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

### Currying
```js
const finalPriceCurried = (discount) => (price) =>  price - ((discount/100) * price); 

const nonPrimeMemberPrice = finalPriceCurried(40);
const primeMemberPrice = finalPriceCurried(50);

nonPrimeMemberPrice(500) // 300
primeMemberPrice(500) //
```

#### Resources 
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


