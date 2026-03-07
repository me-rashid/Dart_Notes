
# 🚀 Dart Operators & Control Flow 

---

# 🟢 Operators in Dart

```dart
// Operator se hume Dart programming me bohat asani milti hai.
```

---

## 🔹 Types of Operators

```dart
// Arithmetic Operators  = ( +, -, *, /, %, ~/ )
// Relational Operators  = ( ==, !=, >, <, >=, <= )
// Logical Operators     = ( &&, ||, ! )
// Assignment Operators
// Increment / Decrement
```

👉 In ke ilawa aur bhi operators hain, lekin Dart me ye zyada use hote hain.

---

# 🟢 Arithmetic Operators

```
( +, -, *, /, %, ~/ )
```

---

## 🔹 BODMAS Rule Example

```
2 + 3 / 4 + 5 - 2 * (2 + 3)

Step by Step:
2 + 3 / 4 + 5 - 2 * 5
2 + 0.75 + 5 - 10
2.75 + 5 - 10
7.75 - 10
-2.25
```

---

## 🔹 Examples

```dart
print(1 + 2);   // 3  ---> Addition
print(3 - 2);   // 1  ---> Subtraction
print(3 * 4);   // 12 ---> Multiplication
```

---

### Division

```dart
print(7 / 2);   // 3.5  (double)
print(4 / 2);   // 2.0  (double)
```

👉 `/` hamesha double return karta hai.

---

### Integer Division

```dart
print(7 ~/ 2);  // 3  (int)
print(4 ~/ 2);  // 2  (int)
```

👉 `~/` decimal remove karta hai.

---

### Modulus

```dart
print(7 % 2);   // 1  (remainder)
```

---

# 🟢 Relational Operators

```
( ==, !=, >, <, >=, <= )
```

---

```dart
print(5 == 5);   // true
print(4 == 5);   // false
```

👉 `==` check karta hai barabar hai ya nahi.

---

```dart
print(5 != 5);   // false
```

👉 `!=` check karta hai barabar nahi hai.

---

```dart
print(1 > 3);    // false
print(1 < 3);    // true
```

---

```dart
print(33 >= 5);  // true
print(33 <= 5);  // false
```

---

# 🟢 Logical Operators

```
( && , || , ! )
AND , OR , NOT
```

---

## 🔹 NOT (!)

```dart
print(!true);   // false
print(!false);  // true
```

👉 `!` value ko opposite kar deta hai.

---

## 🔹 AND (&&)

👉 Dono values true hongi tabhi result true hoga.

```dart
bool a = true;
bool b = true;
print(a && b);  // true
```

```dart
bool a = true;
bool b = false;
print(a && b);  // false
```

---

## 🔹 OR (||)

👉 Agar aik bhi value true ho to result true hoga.

```dart
bool a = true;
bool b = false;
print(a || b);  // true
```

```dart
bool a = false;
bool b = false;
print(a || b);  // false
```

---

# 🟢 Assignment Operator

```dart
int a = 5;   // Assignment
a = 6;       // Re-assignment
```

👉 Variable me value assign karna assignment kehlata hai.

---

# 🟢 Increment / Decrement

```
++   ---> Increment
--   ---> Decrement
```

---

```dart
int y = 5;
print(y);  // 5
```

---

## 🔹 Post Increment

```dart
print(y++);  // 5
print(y);    // 6
```

👉 Pehle print karega, baad me increment karega.

---

## 🔹 Pre Increment

```dart
print(++y);  // 6
```

👉 Pehle increment karega, phir print karega.

---

# 🟢 Control Flow

```
if / else
```

---

## 🔹 Simple If

```dart
if (1 == 1) {
  print("yes it is true");
}
```

👉 Agar condition true ho to print chalega.

---

```dart
if (1 == 2) {
  print("yes it is true");
}
```

👉 Condition false hai, kuch print nahi hoga.

---

## 🔹 If / Else

```dart
if (1 == 1) {
  print("true");
} else {
  print("no true");
}
```

---

```dart
if (1 == 2) {
  print("true");
} else {
  print("no true");
}
```

---

## 🔹 Variables ke through

```dart
int y = 5;
int z = 7;

if (y > z) {
  print("true");
} else {
  print("no true");
}
```

👉 5, 7 se bara nahi hai, is liye else chalega.

---

# 🟢 Switch Statement

```dart
int day = 3;

switch (day) {
  case 1:
    print("Monday");
    break;

  case 2:
    print("Tuesday");
    break;

  case 3:
    print("Wednesday");
    break;

  case 4:
    print("Thursday");
    break;

  default:
    print("Default");
}
```

👉 Day = 3 hai, is liye Wednesday print hoga.

---

# 🟢 Ternary Operator

```dart
var result = (1 == 1) ? "yes" : "no";
print(result);  // yes
```

👉 Short form of if/else.

---

# 🟢 Null Safety Operator

---

## 🔹 Null Aware (?.) & Null Coalescing (??)

```dart
String? a = null;
print(a?.length ?? "hey there is no data");
```

Output:

```
hey there is no data
```

👉 Agar left side null ho to `??` wali value print hogi.

---

```dart
String? a = "rashid";
print(a?.length ?? "hey there is no data");
```

Output:

```
6
```

👉 Yahan value null nahi hai, is liye length print hogi.

---

# 🎯 Important Points

* Arithmetic operators math ke liye use hote hain
* Relational operators comparison ke liye
* Logical operators boolean ke liye
* Increment / Decrement important hain
* if/else decision making ke liye
* switch multiple conditions ke liye
* ternary short if/else hai
* `??` null handle karta hai

---

