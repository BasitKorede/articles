# CONDITIONAL STATEMENT IN JAVASCRIPT.

Conditional statements are statements that perform particular tasks based on the given condition(s).

## This project explains the following:

- What conditional statements are.
- The `if` statement.
- The `if...else` statement.
- Logical operators.
- ternary operators.
- Truthy and falsy.
- Truthy and falsy assignment.
- The `else...if` statement.
- Switch keyword.

## The `if` statement:

Tasks are mostly carried out based on condition. For example, if you are hungry, then you will eat. If it rains, then you use your umbrella.

The same thing applies to our code . in javascript we use the `if` statement to perform tasks based on conditions.

```js
let  bestScore = 40;
if (bestScore <= 45);{
console.log(" please play again")
}
\\ prints: Please play again.
```

If the condition `(bestscore <= 45)` which means bestScore should be less than or equals to 45 to evaluates to `true`, Which means the code in the curly braces would run, but if it greater than 45 that means it will evaluate to `false`. Leaving the condition unevaluated. Therefore if the condition evaluates to `true` it would log `\\ Please play again` to the console.

## The `if...else` Statement:

The `if...else` statement is used when adding another condition in case to the statement. Meaning if the condition evaluates to false the other condition will run.

```js
let workingDays = 4;
if (workingDays === 5) {
    console.log('Thanks for your commitment');
}else{
    console.log('you were absent!');
}
\\ Prints: You were absent!.
```

## Logical Operators:

Using conditional statements means using `true` or `false` and `boolean`.
In javascript there are operators used with boolean known as logical operators. They add more logical expression to our conditions. We have three types of logical operators:

- The and operator ( && ).
- The or operator ( | | ).
- The not operator also known as the bang
  operator ( ! ).

The `and` ( && ) operator: the `and` operator is used to check if the two conditions are `true`.

```js
if (weekDays === "sunday" && time === "12:00pm") {
  console.log("it sunday afternoon");
} else {
  console.log("not aternoon yet");
}
```

When using the `and` operator the statement only evaluate to `true` only when both of the conditions are `true`. If one of the condition evaluates to `false`, the second code block runs.

The `or` ( | | ) operator: the `or` operator is use to check if one of the conditions is `true`.

example:

```js
if (firstName === "basit" || firstname === "korede") {
  console.log("Identified user");
} else {
  console.log("Unidentified user");
}
```

When using the `or` operator, the statement evaluates
to `true` when only one of the conditions is `true`.
In the statement above, the overall statement will evaluate to false only when both the condition are `false`.

## Ternary operators:

The ternary operator is basically used to simplify an
`if ... else` statement. It works like an `if ...else` statement, but shorter and easier to use.

example:
We have our `if ...else` statement.

```js
if (pizza === "dough") {
  console.log("pizza is made with dough");
} else {
  console.log("pizza is not made with dough");
}
```

Ternary operation can also be used to carry out same functionality.

```js
pizza === "dough"
  ? console.log("pizza iis madewith dough")
  : console.log("pizza is not made with dough");
```

When using the ternary operator, the condition should be passed before the (`?`) then followed by the expressions, which are also separated with a (`:`) column. Then the first expression evaluates as `true`, and the second as `false`.

## Truthy and Falsy:

Sometimes, we check if variable exist, and we don't necessarily what it to equal to a specific value. We just want to check if it has been assigned a value.

example:

```js
let firstName = "basit";
if (firstName) {
  console.log("that is my first name");
} else {
  console.log("firstName not defined");
}
```

The code block `if` will run, because `firstName` evaluates to `true`, even though the value `firstname` has not been given the value of `true`. a statement evaluates to `true` when it has not been assigned a `falsy` value.
list of falsy values are:

- 0
- An empty string "" or ''
- Null, which means there is no value at all.
- Undefined, which means a declared variable has not be assigned a value.
- NaN, which stands for not a number.

Example :

```js
let numberOfStudent = 0;
if numberOfStundent0{
  console.log('there are some student left');
}else{
  console.log("there is no student left");
}
```

In the statement above the `if` code block evaluates to `false` because it has been assigned a `falsy` value. So the `else` block will run.

`\\` prints: there is no student left.

## Truthy and Falsy Assignment:

The truthy and falsy assignment also allows shorthand possibilities.
The below expressions checks if a particular store has default goods.

```js
let defaultGoods;
if (defaultGoods) {
  defaultGoods = "";
  console.log("Rice");
} else {
  console.log("No default goods");
}
```

The above statement logs out `\\` No default goods.
Because the variable `defaultGoods` is undefined so it `falsy` and the `false` condition takes precedence.
The above statement can also be written as.

```js
defaultGoods = "rice" || "No default goods";
```

This statement checks if DefaultGoods is assigned a value. Then continue to check from left `if` the statement is `true`, `else` goes on to check the right condition and evalutes it if the statement is `false`.

## The `Else ...If` Statement:

The `else ...if` statement allows us to and more conditions to our `if ...else` statement. With the `else ...if` statement we can have more than two possible outcomes. We can have as many `else ...if` statement as possible.

example:

```js
let poultryAnimal = 'turkey';
if (poultryAnimal === 'chicken'){
  console.log('enjoy your chicken')
}else if (poultryAnimal ==='waterfowl'){
  console.log('enjoy your waterfowl')
}
else if (poultryAnimal === 'ducks'){
  console.log('enjoy your ducks')
}else{
  console.log('Consider adding turkey to your cart')
}
\\ prints: Consider adding turkey to your cart
```

The `else ...if` statement allows the adding of more conditions to our statement.

## The Switch Keyword:

The switch keyword is used like the `else ...if` statement, but with more simplicity. In programming, we often need to check multiple conditions. Also often need to treat their values differently.
example:

```js
let grain = 'Rice'
if (grain = 'Barly'){
  console.log('barly now cost £1.00 per Kg')
  }else if (grain = 'Oat'){
  console.log('oat now cost £0.7 per Kg')
  }else if (grain = 'Wheat'){
  console.log('wheat now cost £2.00 per Kg')
  }else if (grain = 'Corn'){
  console.log('corn now cost £0.7 per Kg')
 } else if (grain = 'Rice'){
  console.log('Rice now cost £1.00 per Kg')
}else{
 console.log('Unknown grain')
}
```
In the above code, we have different conditions, and our code works fine. 
The switch keyword would be of help in a situation. Whereby we are entering hundred of values in our code.
It simplify, and eases us from stress.

example:
```js
let grain = 'Rice'
switch (grain) {
  case 'Barley':
  console.log('barely now cost £1.00 per Kg')
   break;

  case  'Oat':
  console.log('oat now cost £0.7 per Kg')
  break;

  case 'Wheat':
  console.log('wheat now cost £2.00 per Kg')
  break;

  case 'Corn':
  console.log('corn now cost £0.7 per Kg')
  break;

  case 'Rice':
  console.log('Rice now cost £1.00 per Kg')
   break;

   default:
 console.log('Unknown grain')
 break;
}
```
- The `switch` keyword initiates the statement, followed by a parenthesis `(...)`. Which contains the value that will be compared by each `case`.
- The `case` keyword checks if the expression matches the specific value that comes after it. It checks all the conditions, and logs out the one the value is equal to the value of the variable.
- The `break` keyword tells the computer to exit the block and not execute any more code from the code block. Or check if there are other cases in the block.
- The `default` statement works like our `else` statement. It runs in cases where our `case`(s) does not evaluate to `true`. 

 


