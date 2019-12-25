# Conditional Statements

### If-Then-Else

---

## Agenda

@ol
* Basic `if` statement syntaxs
* Ternary Operator
@olend

---

## Basic `if else` statement syntax 1

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

if (vat > 0.0) {
	amount = price * (100 + vat) / 100;
} else {
	amount = price;
}
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

---

## Basic `if` statement syntax 2

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

---

## Basic `else if` statement syntax 3

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

---

## Basic `if if` statement syntax 3

```csharp
if (condition) {

} if (condition) {

} if (condition) {

} else {

}
```

+++

## demo 1

```csharp
if (score > 80) {
	grade = "A";
} if (score > 70) {
	grade = "B";
} if (score > 60) {
	grade = "C";
} else {
	grade = "F";
}
```

---

## Basic `if in if` statement syntax 3

```csharp
if (condition) {

	if (condition) {

	} else (

	)
}
```

+++

## demo 1

```csharp
if (a == 1) {

	if (b == 2) {
		Console.writeline("Hello World")
	} else (
		Console.writeline("Hello mama");
	)
}
```

---

## Ternary Operator

```csharp
result = condition ? valueIfTrue: valueIfFalse;
```

+++

## demo 1

```csharp
amount = vat > 0.0 ? price * (100 + vat) / 100 : price;
```

+++

## demo 2

