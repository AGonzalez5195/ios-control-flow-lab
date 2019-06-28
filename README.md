# Control Flow Lab

## Question 1

What will be printed when the code below is run?  Select all that apply.

```swift
let conditionOne = !(4 < 5) || !(3 > 8)
let conditionTwo = !(!true)

if conditionOne {
 print("A")
} else if conditionTwo {
 print("B")
}
if conditionTwo {
 print("C")
}
print("D")
```
((A))
-B
((C))
((D))

B isn't printed because it's dependent on A not being true, which it is. Thus, the computer does not even procede to the next step after A.
***
## Question 2

What will the code block below print?  Select all that apply:

```swift
let appInfo = (name: "myCoolApp", version: 0.4)
switch appInfo {
 case (_, 0.0..<1.0):
 print("\(appInfo.0) hasn't released yet")
 case ("myCoolApp", _):
 print("Thanks for looking at myCoolApp!")
 default:
 print("I'm not quite sure what you are looking at")
}
```

- appInfo.0 hasn't released yet
- ((myCoolApp hasn't released yet))
- Thanks for looking at myCoolApp!
- I'm not quite sure what you are looking at
- It will give a compile-time error


myCoolApp is the only message that will display. This is because the first case (_, 0.0 .. <1.0) is satisfied since the version in the appInfo tuple is given as 0.4. None of the other lines will be printed since the conditions aren't met.
***
## Question 3

What will be printed to the console when the code below is run?  Select all that apply.

```swift
let x: Int = 4
switch x {
case 0..<4:
 print("A")
case 5..<10:
 print("B")
case is Double:
 print("C")
default:
 print("D")
}
```

- A
- B
- C
- ((D))

The integer 4 is not in the range of 0 and 4 with 4 being unincluded. Therefore, A is out. It is also not in between the range of 5 and 10 so B is out. It is not of the type Double so C is out. This leaves D, which is the default that encompasses all else.
***
## Question 4

What are the errors in the code below for the switch statement? Select all that apply.

```swift
let candyType : String = "skittles"

switch candyType {
case "mAndM":
 print("Melts in your mouth, not in your hand")
case "skittles":
 print("Taste the rainbow")
case "snickers":
 print("Hungry? Grab a Snickers")
}
```

- No parentheses around the conditions
- No opening and closing brackets in each of the cases
- ((No default case in the switch statement))
- No print statement right outside the switch statement

There is no default case in the switch statement so it is not exhaustive. The other answers aren't relevant.
***
## Question 5

Given the current weather conditions (rain, sunny, snow), use a switch statement to print an appropriate message to the user

```swift
let currentWeather = "rain"

// enter code below

switch currentWeather {
case "rain":
    print("It's raining")
case "snow":
    print("It's snowing")
case "sunny":
    print("It's sunny")
default:
    print("It's neither raining, snowy, or sunny")
}

```

***
## Question 6

Given the first name and last name of a Fellow, declare `fullName` variable and use string interpolation to concatenate the Fellow's full name and print to the console e.g The Fellow's full name is John Appleseed

```swift
let firstName = "John"
let lastName = "Appleseed"

// enter code below

var fullName = firstName + " " + lastName
print ("The Fellow's full name is " + fullName)

```

***
