
---

# 🟢 Flutter & Dart

```dart
// Dart --> Flutter
// Flutter Dart se bana hai.
// Flutter se hum mobile applications banate hain.
// Dart Flutter ki official language hai.
// Flutter Dart ko understand karta hai.
```

---

# 🟢 DartPad

```dart
// DartPad =
// DartPad aik online compiler hai jahan hum Dart code likh kar run kar sakte hain.
// Is ke liye system me Dart install karne ki zarurat nahi hoti.
// Browser me hi code likh kar output dekh sakte hain.
```

---

# 🟢 Dart Kya Hai?

```dart
// Dart aik language hai.
// Hum insaan ek doosre se language ke zariye baat karte hain
// jaise Urdu, Pashto, English.

// Isi tarah jab hum computer se baat karte hain
// to programming language use karte hain.

// Computer Urdu ya English nahi samajhta.
// Computer sirf 010101 (binary) samajhta hai.

// Hum 010101 yaad nahi kar sakte.
// Is liye programming languages banayi gayi.
// Dart bhi un me se aik language hai.
```

---

# 🟢 Main Function (Entry Point)

```dart
void main() {

}
```

```dart
// main() Dart program ka entry point hai.
// Jab bhi program run hota hai
// sabse pehle main() function run hota hai.

// Sirf main function ke andar likha code run hota hai.
// Agar koi aur function ho aur usko call na karein
// to wo run nahi hoga.

// Main aik scope ki tarah kaam karta hai.
```

---

### Example

```dart
void main() {
  int a = 1;
  print(a); // Output = 1
}
```

---

# 🟢 Keywords

```dart
// Keywords wo special words hote hain
// jo Dart me pehle se defined hote hain.

// Inka apna special meaning hota hai.

// Examples:
void
main
print
int
double
String
bool

// In keywords ko hum variable name ke tor par use nahi kar sakte.
```

---

# 🟢 Print

```dart
void main() {
  print("Hi I am Rashid");
}
```

Output:

```
Hi I am Rashid
```

---

## 🔹 Important Rules of print()

```dart
// print() ko kam az kam aik value deni zaroori hoti hai.
// Agar empty print() likhenge to error aayega.

// print();  // Error
// print("Hello"); // Correct
```

---

# 🟢 Difference Between Number & String

```dart
print(3);     // 3  (yeh number hai)
print("3");   // 3  (yeh string hai)
```

👉 Dono same lagte hain
Lekin datatype different hai.

---

### Example

```dart
print(3 + 2);        // 5
print("3" + "2");    // 32
// print(3 + "2");   // Error
```

👉 Number + Number = Addition
👉 String + String = Concatenation

---

# 🟢 Concatenation

```dart
print("Hi " + "Rashid"); // Hi Rashid
```

⚠ Dart me sirf `+` operator string ke liye use hota hai.
`- * / %` string par use nahi kar sakte.

```dart
// print("3" * 2);  // Error in Dart
```

---

# 🟢 BODMAS Rule

```dart
// Dart BODMAS rule follow karta hai.

// B = Brackets
// O = Orders
// D = Division
// M = Multiplication
// A = Addition
// S = Subtraction
```

Example:

```dart
print(2 + 3 * 2); // 8
```

Explanation:

```
3 * 2 = 6
2 + 6 = 8
```

---

# 🟢 Comments

## 1️⃣ Single Line Comment

```dart
// this is comment
```

## 2️⃣ Multi-line Comment

```dart
/*
   this is comment
   this is comment
*/
```

## 3️⃣ Documentation Comment

```dart
/// this is documentation comment
```

---

# 🟢 Error

```dart
// Error ka matlab hai ghalti.
// Jab code galat hoga Dart hume error dega.
// Error se hume pata chalta hai ke code me problem hai.
```

---

# 🟢 Semicolon ;

```dart
// Jab line khatam hoti hai
// to end me ; lagate hain.
```

Example:

```dart
int a = 5;
```

---

# 🟢 Functions Example

```dart
void main() {
  print("my name is muhammad");
}

void lolo() {
  print("my name is jabir");
}
```

Output:

```
my name is muhammad
```

👉 Sirf main() run hota hai.

---
