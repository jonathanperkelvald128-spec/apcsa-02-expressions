# Exercise 11 — The Debugging Gauntlet

Five programs, escalating difficulty. Fix each one, then document it.

For each: what type of error, what the message said (or didn't), and what was actually wrong.

---

## DebugMe1

| | |
|---|---|
| **Error** | Synatx |
| **Message** |src/DebugMe2.java:6 error `;' expected, and src/D
 |
| **What was actually wrong** |Missing a semicolon |
| **The fix** | adding a semicolon |

---

## DebugMe2

| | |
|---|---|
| **Error type** |Syntax and type errors |
| **Message** | String cannot be converted to message |
| **What was wrong** | The age was written as text ("17") instead of a number (17).|
| **The fix** | Remove the quotations and add a semicolon |

---

## DebugMe3

| | |
|---|---|
| **Error type** |Type error |
| **Message** | double cant be converted to int|
| **What was wrong** |A decimal was stored in an integer  |
| **The fix** | Change int rounded = price; to int rounded = (int) price;|

---

## DebugMe4

| | |
|---|---|
| **Error type** | Case sensitivity error|
| **Message** | cannot find symbol|
| **What was wrong** |totalscore and Average have the wrong capitalization. |
| **The fix** | totalscore to totalScore and Average to average.|

---

## DebugMe5

> ⚠️ This one **compiles and runs**. It just gives the wrong answer.

| | |
|---|---|
| **Error type** | Logic error|
| **What output did you expect?** |86.0 % |
| **What output did you get?** | 0.0%|
| **What was actually wrong** | Java divided two integers, giving 0.|
| **The fix** | change to double percentage = (double) pointsEarned / pointsPossible * 100;|
| **How did you find it?** | I checked the division and found that it gave 0 instead of a decimal.|

---

## Reflection

**1. Which was hardest? Why?**

[DebugMe5 was hardest because the code ran but gave the wrong answer.]

**2. DebugMe5 had no error message at all. What strategy did you use to find the problem?**

[I checked the math and looked at the values to find the mistake.]

**3. Why is a logic error more dangerous in real software than a syntax error?**

[A logic error is more dangerous because the program runs but gives wrong results without warning.]
