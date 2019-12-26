## If & if-else

---

## Agenda

@ol
* `if-else` Statement Syntaxs
* `if` Statement Syntaxs

@olend

---
##  `if else` Statement Syntax 

```csharp
if (condition) 
{
// Do if the condition is true
} 
else 
{
// Or if the condition is not met
}
```

+++

## Demo 1

```csharp
var name = "John";

if (name == "John") 
{
	Console.WriteLine("Oh, I'm looking for you John!");
} 
else 
{
	Console.WriteLine("Sorry, I thought you're John.");
}
```

 #### result

```csharp
Oh, I'm looking for you John!
```

+++

## Demo 2

```csharp
var name = "Joe";

if (name == "John") 
{
	Console.WriteLine("Oh, I'm looking for you John!");
} 
else 
{
	Console.WriteLine("Sorry, I thought you're John.");
}
```

#### result

```csharp
Sorry, I thought you're John.
```

---
##  `if` Statement Syntax 

```csharp
if (condition) 
{
// Do if the condition is true
}
```

+++

## Demo 1

```csharp
var name = "John";

if (name == "John") 
{
	Console.WriteLine("Oh, I'm looking for you John!");
}
Console.WriteLine("Sorry, I thought you're John.");
```

#### result

```csharp
Oh, I'm looking for you John!
Sorry, I thought you're John.
```
##### ถึง name จะเป็นจริงหรือไม่ *"Sorry, I thought you're John."* ยังแสดงผลอยู่ดี
