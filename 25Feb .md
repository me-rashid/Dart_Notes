

# 🟢 Variables

```dart
// Variable wo cheez hoti hai jo change ho sakti hai.
// Variable ek container hai jahan hum value store karte hain.
```

---

## 🔹 Structure

```
datatype variableName = value;
```

---

# 🟢 Data Types

| No | Data Type | Example      |
| -- | --------- | ------------ |
| 1  | int       | 1, 2, 3      |
| 2  | double    | 1.5, 2.3     |
| 3  | String    | "hi"         |
| 4  | bool      | true / false |

---

# 🟢 Example Variables

```dart
int phoneNumber = 3709630467;
String cityLocation = "hi";
double age = 16.5;
bool isPresent = true;
```

---

# 🟢 Print Variables

```dart
print(phoneNumber);
print(cityLocation);
print(age);
print(isPresent);
```

---

# 🟢 Print All Together

```dart
print("$phoneNumber $cityLocation $age $isPresent");
```

---

# 🟢 Advantage of Variables (Very Important)

```dart
// Agar hum koi value multiple jagah use kar rahe hain
// aur baad me us value ko change karna ho
// to hume har jagah manually change nahi karna padega.

// Sirf variable ki value aik jagah change karenge
// aur jaha jaha use hoga sab jagah reflect hoga.
```

Example:

```dart
var age = 5;

print(age * 3); // 15
print(age + 4); // 9

age = 9; // value changed
```

---

# 🟢 Changing Variable Value

```dart
String a = "hi Muhammad";

a = "hi"; // Correct
```

❌ Wrong:

```dart
// a = 20; // Error (datatype change nahi kar sakte)
```

---

# 🟢 Dynamic

```dart
// Dynamic wo hota hai jisme har type ki value assign ki ja sakti hai.
// Compiler compile time par type check nahi karta.
```

---

## 🔹 Example 1

```dart
dynamic c = "hi Muhammad";
print(c.runtimeType);
```

Output:

```
String
```

👉 Yahan error nahi aaya
Kyuki variable dynamic hai.

---

## 🔹 Value Change Example

```dart
dynamic c = "hi";
print(c.runtimeType);   // String

c = 2;
print(c.runtimeType);   // int

c = 1.3;
print(c.runtimeType);   // double

c = true;
print(c.runtimeType);   // bool
```

👉 Dynamic me datatype change ho sakta hai.
👉 `runtimeType` runtime par actual object ka type batata hai.
👉 Compiler compile time par type check nahi karta.

---

## ⚠ Important Note

Dynamic compile time par type check nahi karta.
Actual datatype runtime par object ka hota hai.

Is wajah se:

• Proper compile time safety nahi milti
• IDE full type suggestions nahi deta
• Large projects me bugs ka risk barh jata hai

👉 Production code me dynamic avoid karna chahiye jab tak zarurat na ho.

---

# 🟢 Dot (.) Operator

Dot (.) operator ka use datatype ki properties aur methods access karne ke liye hota hai.

---

## 🔹 Example (int properties)

```dart
int marks = 30;

print(marks.isNegative); // false
print(marks.isEven);     // true
```

👉 `isNegative` aur `isEven` int ki properties hain.
👉 Har datatype ki apni properties aur methods hoti hain.

---

## 🔹 Example (String properties)

```dart
String city = "Hangu";

print(city.endsWith("u"));
```

Output:

```
true
```

👉 `endsWith` check karta hai ke string ka last letter kya hai.

---

## 🔹 Dynamic ke saath

```dart
dynamic marks = 30;
print(marks.);
```

👉 Dynamic me compile time par type unknown hota hai
isliye proper type safety aur full suggestions nahi milti.

---

# 🟢 Var

```dart
// Var me Dart automatically datatype detect karta hai.
```

---

## 🔹 Example

```dart
var a = 10;

a = 20;     // ✔ allowed
a = "10";   // ❌ Error
```

👉 Var first assigned value se datatype detect karta hai.
👉 Baad me datatype change nahi hota.
👉 Var mutable hota hai (value change ho sakti hai).

---

## 🟡 Type Inference

Var, final aur const me Dart automatically datatype detect karta hai.
Is process ko **Type Inference** kehte hain.

Example:

```dart
var a = 10;   // Dart ne khud detect kiya ke ye int hai
```

---

# 🟢 Final

```dart
// Final ki value sirf ek baar assign hoti hai.
// Assign hone ke baad change nahi hoti.
```

---

## 🔹 Example

```dart
final a = 4;

a = 5; // ❌ Error
```

👉 Final runtime par value le sakta hai.
👉 Lekin ek baar assign hone ke baad dobara change nahi hota.

---

# 🟢 Const (Constant)

```dart
// Const compile time constant hota hai.
// Value compile time par hi known honi chahiye.
```

👉 Const ki value completely fixed hoti hai.
👉 Runtime value assign nahi kar sakte.

---

## 🟡 Real Difference Example

```dart
final timeNow = DateTime.now();   // ✔ allowed
const timeNow = DateTime.now();   // ❌ error
```

Kyuki:

• `DateTime.now()` runtime par value deta hai
• Const ko compile time par known value chahiye hoti hai

---

