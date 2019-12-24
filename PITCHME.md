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

## Quick Demo I

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

---

@title[Code]

```
// Include http module.
var http = require("http");
// Create the server. Function passed as parameter
// is called on every request made.
http.createServer(function (request, response) {
  // Attach listener on end event.  This event is
  // called when client sent, awaiting response.
  request.on("end", function () {
    // Write headers to the response.
    // HTTP 200 status, Content-Type text/plain.
    response.writeHead(200, {
      'Content-Type': 'text/plain'
    });
    // Send data and end response.
    response.end('Hello HTTP!');
  });
// Listen on the 8080 port.
}).listen(8080);
```

@[1,2](You can present code inlined within your slide markdown too.)
@[9-17](Your code is displayed using code-syntax highlighting just like your IDE.)
@[19-20](Again, all of this without ever leaving your slideshow.)
