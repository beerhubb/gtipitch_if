# Conditional Statements

### If-Then-Else, Switch-Case

---

## Agenda

* Basic `if` statement syntaxs
* Ternary Operator
* Demo

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

## Quick Demo

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

## Demo I

```csharp
var name = Console.ReadLine();

if (name == "John") {
	Console.WriteLine("Oh, I'm looking for you John!");
} else {
	Console.WriteLine("Sorry, I thought you're John.");
}
```

+++

## Demo II

```csharp
var name = Console.ReadLine();

if (name == "John") {
	Console.WriteLine("Oh, I'm looking for you John!");
}
Console.WriteLine("Sorry, I thought you're John.");
```

+++

## Demo III

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
```

+++

## Demo IV

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

+++

## Demo V

```csharp
if (score > 60) {
	grade = "A";
} else if (score > 70) {
	grade = "B";
} else if (score > 80) {
	grade = "C";
} else {
	grade = "F";
}
```

+++

## Quiz I

Could you rewrite conditional in `Demo V` to work exactly like `Demo III`?

+++

## Quiz II

What structure do we use to compute the number of bank notes and coins?

+++

## Quiz III

How to set `file2open` to *"inputfi.csv"* when `fname` is null?

```csharp
void OpenInputFile(string fname) {
	// ...
	string file2open;
	// ...
	// Process `file2open`
}
```

+++

## Demo VI

```csharp
void OpenInputFile(string fname) {
	string file2open;

	if (fname == null) {
		file2open = "inputfi.csv";
	} else {
		file2open = fname;
	}
	// Process `file2open`
}
```

+++

## Demo VII

```csharp
void OpenInputFile(string fname) {
	string file2open = fname;

	if (fname == null) {
		file2open = "inputfi.csv";
	}
	// Process `file2open`
}
```

+++

## Demo VIII

```csharp
void OpenInputFile(string fname) {
	string file2open = (fname == null)
		? "inputfi.csv"
		: fname;
	// Process `file2open`
}
```

---

## Null-Coalescing Operator (??)

```csharp
var targetVar = targetValue ?? fallbackValue;
```

+++

## Demo IX

```csharp
void OpenInputFile(string fname) {
	string file2open = fname ?? "inputfi.csv";
	// Process `file2open`
}
```

+++

## Quiz IV

How to set `file2open` to *"inputfi.csv"* when `fname` is null **or has only whitespace**?

```csharp
void OpenInputFile(string fname) {
	// ...
	string file2open;
	// ...
	// Process `file2open`
}
```

+++

## Demo X

```csharp
void OpenInputFile(string fname) {
	string file2open = string.IsNullOrWhiteSpace(fname)
		? "inputfi.csv"
		: fname;
	// Process `file2open`
}
```

+++

## Demo XI

```csharp
void OpenInputFile(string fname) {
	string file2open = fname;

	if (string.IsNullOrWhiteSpace(fname)) {
		file2open = "inputfi.csv";
	}
	// Process `file2open`
}
```

---

## Quiz V

How to get the number of elements in `inputData` and assign to `count` correctly?

```csharp
void ComputeMean(int[] inputData) {
	// How to set this variable correctly.
	var count;
}
```

+++

## Demo XII

```csharp
void ComputeMean(int[] inputData) {
	var count;
	if (inputData != null) {
		count = inputData.Length;
	}
}
```

+++

## Demo XIII

```csharp
void ComputeMean(int[] inputData) {
	var count = 0;
	if (inputData != null) {
		count = inputData.Length;
	}
}
```

---

## Null-Conditional Operators

### ?. and ?[]

```csharp
var count = inputData?.Length;
```

+++

## Demo XIV

```csharp
void ComputeMean(int[] inputData) {
	var count = inputData?.Length;
}
```

+++

## Demo XV

```csharp
void ComputeMean(int[] inputData) {
	var count = inputData?.Length ?? 0;
}
```
