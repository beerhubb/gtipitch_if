# Conditional Statements

### If-Then-Else

---

## Agenda

@ol
* Basic `if` statement syntaxs
* Ternary Operator
* Demo
@olend

---

## Basic `if` statement syntax I

```csharp
if (condition) {
	// Do if the condition is true
} else {
	// Or if the condition is not met
}
```

+++

## Basic `if` statement syntax II

```csharp
if (condition) {
	// Do if the condition is true
}
```

+++

## Basic `if` statement syntax III

```csharp
if (condition) {
	// Do if the condition is true
} else if(condition2) {
	// Do if not met the first condition
	// but the 2nd one is true
} else {
	// Or if those above conditions are not met
}
```

---

## Quick Demo

```csharp
vat = 7.0; // VAT 7%

if (vat > 0.0) {
	amount = price * (100 + vat) / 100;
} else {
	amount = price;
}
```

---

## Ternary Operator

```csharp
result = condition ? valueIfTrue: valueIfFalse;
```

+++

## Ternary Operator

```csharp
amount = vat > 0.0 ? price * (100 + vat) / 100 : price;
```

+++

## Quick Demo 1

```csharp
vat = 7.0; // VAT 7%

if (vat > 0.0) {
	amount = price * (100 + vat) / 100;
} else {
	amount = price;
}
```

v.s.

```csharp
amount = (vat > 0.0) ? price * (100 + vat) / 100 : price;
```

---

## Demo 1

```csharp
var name = Console.ReadLine();

if (name == "John") {
	Console.WriteLine("Oh, I'm looking for you John!");
} else {
	Console.WriteLine("Sorry, I thought you're John.");
}
```

+++

## Demo 2

```csharp
var name = Console.ReadLine();

if (name == "John") {
	Console.WriteLine("Oh, I'm looking for you John!");
}
Console.WriteLine("Sorry, I thought you're John.");
```

+++

## Demo 3

```csharp
if (score > 80) {
	grade = "A";
} else if (score > 70) {
	grade = "B";
} else if (score > 60) {
	grade = "C";
} else {
	grade = "F";
}
---
## Example

```
Normal cases
1.ผู้ใช้กดเงินออกจากตู้ข้อมูลถูกต้อง ระบบทำการหักเงินแล้วนำเงินออกมา
2.ผู้ใช้กดเงินออกจากตู้แต่เงินในบัญชีไม่พอ ระบบทำการแจ้งเตือน
3.ผู้ใช้กดเงินออกจากตู้ข้อมูลถูกต้อง แต่ตู้มีเงินไม่พอจ่าย ระบบทำการแจ้งเตือน

Alternative cases
4.ผู้ใช้บัญชีพิเศษกดเงินมากกว่าที่มีในบัญชี ระบบบันทึกเครดิตแล้วนำเงินออกมา
5.ผู้ใช้บัญชีพิเศษกดเงินมากกว่าที่มีในบัญชี แต่เครดิตเต็มแล้ว ระบบทำการแจ้งเตือน

Exception cases
6.ผู้ใช้ถอนเงินสำเร็จแต่ระบบไม่สามารถตัดเงินออกจากบัญชีได้ ระบบทำการแจ้งเตือน
```
@[1-4](Normal cases: กรณีที่เจอได้บ่อยๆ 80~90%)
@[6-8](Alternative cases: กรณีที่นานๆจะเกิดขึ้นที หรือเคสขอบ)
@[10-11](Exception cases: กรณีข้อผิดพลาดที่ยอมรับไม่ได้)
