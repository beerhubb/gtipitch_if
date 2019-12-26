## If && if-Else

---

## Agenda

@ol
* Basic `if` statement syntaxs
* Basic `if-else` statement syntaxs
@olend

---

## Basic `if` statement syntax 

```csharp
if (condition) 
{

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

---

## Basic `if else` statement syntax 

```csharp
if (condition) 
{

} 
else 
{

}
```

+++

## Demo 1

```csharp
vat = 7.0; // VAT 7%
price = 100;

if (vat > 0.0) 
{
	var amount = price * (100 + vat) / 100;
} 
else 
{
	amount = price;
}
```

 #### result

```csharp
107
```

+++

## Demo 2

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
