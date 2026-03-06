
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

# 🟢 Optional / Nullable Variable

```dart
// Nullable variable wo hota hai
// jisme value ya to specific datatype hogi
// ya null hoga.
```

---

## 🔹 Null kya hai?

```dart
// Null ka matlab hai variable me koi value nahi hai.
```

⚠ Important:

```
0 null nahi hai
"" (empty string) null nahi hai
```

Kyuki:

• 0 ek value hai
• "" ek empty string hai (lekin value hai)
• Null ka matlab hai bilkul koi value nahi

---

## 🟡 Null Safety Concept

Dart null-safe language hai.

By default:

Har variable non-nullable hota hai.

Example:

```dart
String name = "Rashid";

name = null; // ❌ Error
```

Nullable banane ke liye `?` use karte hain:

```dart
String? name;
int? age;
```

---

## ⚠ Important

```dart
final a = null;
```

Is case me Dart iska type `Null` infer karega.

Agar future me value assign karni ho to nullable type explicitly likhna zaroori hai:

```dart
String? name;
int? age;
```

---

# 🟢 Optional / Nullable Variables

Optional ya Nullable variable ka matlab:

> Ya to variable ke paas value hogi
> Ya phir uski value `null` hogi

Nullable banane ke liye datatype ke baad `?` lagaya jata hai.

```dart
String? name;
int? age;
```

---

# 🟢 Null kya hai?

Null ka matlab hai:

👉 Variable me bilkul koi value nahi hai.

⚠ Important:

```
0 null nahi hai
"" null nahi hai
"null" null nahi hai
```

• 0 ek value hai
• "" ek empty string hai
• "null" ek string hai
• Null ka matlab hai no value

---

# 🟢 Sound Null Safety (SNS)

Dart me Sound Null Safety hoti hai.

Iska matlab:

👉 Null value par properties access nahi kar sakte.

---

# 🟢 Scope Important Concept

Agar variable `main()` ke andar declare ho
to Dart ko uski value ka pata hota hai.

Lekin agar variable `main()` ke bahar declare ho
to Dart sure nahi hota ke value null hai ya nahi.

Isliye Dart compile time par error deta hai
aur hume force karta hai ke:

• Ya to `?` use karein
• Ya `!` use karein

---

# 🟢 Basic Example

```dart
String? a;

a = "xyz";
print(a.length);  // Error (kyuki nullable hai)

print(a?.length); // Safe
```

---

# 🟢 Null Aware Operator (?.)

```dart
print(a?.length);
```

Matlab:

👉 Agar value null nahi hai to property access karo
👉 Agar null hai to error mat do

---

# 🟢 Null Assertion Operator (!)

```dart
print(a!.length);
```

Matlab:

👉 Hum Dart ko force kar rahe hain
ke variable null nahi hai.

⚠ Agar value actually null hui
to runtime error aayega
aur app crash ho sakti hai.

`!` sirf tab use karein
jab 100% sure ho ke value null nahi hai.

---

# 🟢 Null Coalescing Operator (??)

```dart
print(a?.length ?? "hi user");
```

Matlab:

👉 Agar a null hai to "hi user" print hoga
👉 Agar a null nahi hai to a.length print hoga

Ye user-friendly fallback dene ke liye use hota hai.

---

# 🟢 Example — Error Case

```dart
String? b = null;

print(b.length); // ❌ Error
```

Kyuki null par properties access nahi kar sakte.

---

# 🟢 Example — Safe Case

```dart
String? b = "null";

print(b.length); // 4
```

Yeh actual null nahi hai
Yeh ek string hai.

---

# 🟢 Final Summary

| Operator | Purpose                      |
| -------- | ---------------------------- |
| `?`      | Variable nullable banata hai |
| `?.`     | Safe property access         |
| `!`      | Force non-null (dangerous)   |
| `??`     | Default fallback value       |

---
