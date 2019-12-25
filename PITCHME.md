# Conditional Statements

### If-Then-Else

---

## Agenda

@ol
* Basic `if` statement syntaxs
* Ternary Operator
@olend

---

## Basic `if else` statement syntax 

```csharp
if (condition) {
	// Do if the condition is true
} else {
	// Or if the condition is not met
}
```

+++

## Demo 1

```csharp
vat = 7.0; // VAT 7%
price = 100;

if (vat > 0.0) {
	var amount = price * (100 + vat) / 100;
} else {
	amount = price;
}
```

 ## result

```csharp
 107
```

+++

## Demo 2

```csharp
var name = Console.ReadLine();

if (name == "John") {
	Console.WriteLine("Oh, I'm looking for you John!");
} else {
	Console.WriteLine("Sorry, I thought you're John.");
}
```

## result

```csharp
Oh, I'm looking for you John!
```

```csharp
Sorry, I thought you're John.
```

---

## Basic `if` statement syntax 

```csharp
if (condition) {
	// Do if the condition is true
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

## result

```csharp
Oh, I'm looking for you John!
```
```csharp
Sorry, I thought you're John.
```
##### **ถึง name จะเป็นจริงหรือไม่ *"Sorry, I thought you're John."* ยังแสดงผลอยู่ดีนะ 

---

## Basic `else if` statement syntax 

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

+++

## Demo 3

```csharp
var sccore = 81;

if (score > 80) {
    Console.writeline("A")
} else if (score > 70) {
    Console.writeline("B")
} else if (score > 60) {
    Console.writeline("C")
} else {
    Console.writeline("F")
}
```

## result

```csharp
A
```

---

## Basic `if if` statement syntax 

```csharp
if (condition) {
//
} if (condition) {
//
} if (condition) {
//
} else {
//
}
```

+++

## demo 1

```csharp
var score = 90;
var grade;

if (score > 80) {
	grade = "A";
} if (score > 70) {
	grade = "B";
} if (score > 60) {
	grade = "C";
} else {
	grade = "F";
}
Console.writeline(grade);
```

## result

```csharp
C
```

---

## Basic `if in if` statement syntax 

```csharp
if (condition) {
	if (condition) {
		//
	} else (
		//
	)
}
```

+++

## demo 1

```csharp
var number = 1;
var numbers = 2;
if (number == 1) {

	if (number == 2) {
		Console.writeline("Hello World")
	} else (
		Console.writeline("Hello mama");
	)
}
```

## result

```csharp
Hello World
```

---

## Ternary Operator statement syntax 

```csharp
result = condition ? valueIfTrue: valueIfFalse;
```

+++

## demo 1

```csharp
vat = 0.7;
price = 1000;

amount = vat > 0.0 ? price * (100 + vat) / 100 : price;
```

## result

```csharp
1007
```
