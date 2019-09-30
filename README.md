# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**

Answer
```swift
for q1 in 1..<150 {
    print(q1)
}
```

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

Answer
```swift
for q2 in 142 ..< 160 {
    print(q2)
}
```
***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

Answer
```swift 
for q3 in 15...80 where q3 % 2 == 0 {
    print(q3)
}
```

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

Answer
```swift
for q4 in 19...51 where q4 % 2 == 1 {
    print(q4)
}
```
***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

Answer
```swift
let q5 = 1...100

for q5 in 1..<100 where q5 % 10 == 5 {
    print(q5)
}
```

***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

Answer
```swift
let q6 = 1...40

for q6 in 1...40 where q6 % 10 == 7 {
    print(q6)
}
```

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

Answer
```swift
for q7 in 20..<150 where q7 % 3 == 0 {
    print(q7)
}
```

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

Answer
```swift
for q8 in 20...150 where q8 % 2 == 0 && q8 % 3 == 0 {
    print(q8)
}
```


***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

Answer
```swift
for q9 in 20..<150 where q9 % 10 == 4 {
    print(q9)
}
```

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

Answer
```swift
let q10 = 20...150

for q10 in q10 where q10 == 31 {
    print(q10)
}
for q10 in q10 where q10 == 34 {
print(q10)
}
for q10 in 40...60 {
    print(q10)
}
```
***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

```
Answer
```
The loop will run inifinitely until it crashes, because the i will always be greater than 3, especially when incrementing. Decrementing will correct it.
```
***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
Answer 
```swift
/*
var i = 5

for i in 1 while > 3 && < 9 {
    print(i)
    i += 1
}
*/

// Not sure what function to use here
```
***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
```

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```

# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

Answer
```
Break - will stop the loop once the condition is met
Continue - will proceed with the loop when the condition is met
```

***
## Question 2

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[✅]5 
[✅]6
[]7
[]8
[]9
[]10

***
## Question 3

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[✅]5
[]6
[]7
[]8
[]9
[]10

***
## Question 4

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
```
Answer
```swift
x = 1, y = 2
x = 2, y = 2
x = 3, y = 2
```
***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

***
## Question 7

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```

***
## Question 8

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

***
