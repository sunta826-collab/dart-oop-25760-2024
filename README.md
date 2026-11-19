# Dart OOP Assignment: Kigali Bus Card

**Name:** Mohamed Khalid Gasim
**Student ID:** 25760/2024

## Part 5: Prediction

My prediction:
1
5

Explanation:
The first bag has one item because the setter rejects negative values.
The second bag adds two items each time, then adds one more item.
### Actual Output

1
5

The actual output matches the prediction.
## My numbers

- D = 60
- L = 0
- Starting balance = 1600 RWF
- Bus fare = 260 RWF
- Student discount = 10%

## Output of main.dart

```
Error: name too short
Owner: Mohamed | Balance: 1600 RWF
Owner: Mohamed Khalid Gasim | Balance: 1600 RWF
Error: top-up must be 500 to 50000 RWF
Topped up 2000 RWF
Paid 260 RWF
Paid 260 RWF
Owner: Mohamed Khalid Gasim | Balance: 3080 RWF
Student discount: 26 RWF
Paid 234 RWF
Owner: Mohamed Khalid Gasim | Balance: 1366 RWF
Student card: 10% off
```

## Part 1: Why no setter for balance?

A setter could allow users to change the balance directly.
The balance should only change through topUp and pay.

## Part 2: What does ~/ do?

The ~/ operator returns an integer result.

237 * 17 / 100 = 40.29
237 * 17 ~/ 100 = 40

The first gives a decimal result, while the second removes the decimal part.

## Part 4: Bug table

| Bug | The line | Why it is wrong | My fix |
|---|---|---|---|
| 1 | String _brand; | Fields need initialization. | Added an empty string. |
| 2 | int _battery; | Fields need initialization. | Added 0. |
| 3 | SmartPhone constructor | Parent constructor needs arguments. | Added super(brand, battery). |
| 4 | @override | Parent has no restart method. | Removed @override. |
| 5 | p.battery = 100; and p.battery() | Setter is missing and getter is called like a method. | Added a setter and used p.battery. |
| Not a bug | new Phone | The new keyword is valid in Dart. | No change. |

Bug hunt output: 100