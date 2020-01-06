## if และ if-Else

---

## หัวเรื่อง

* Basic `if` statement syntaxs
* Basic `if-else` statement syntaxs

---

## การใช้ `if` เบื้องต้น

```csharp
if (condition) 
{

}
```

+++

## ตัวอย่างที่ 1

```csharp
var name = "John";

if (name == "John") 
{
	Console.WriteLine("Oh, I'm looking for you John!");
}
Console.WriteLine("Sorry, I thought you're John.");
```

#### ผลลัพธ์

```csharp
Oh, I'm looking for you John!
Sorry, I thought you're John.
```
##### ถึง name จะเป็นจริงหรือไม่ *"Sorry, I thought you're John."* ยังแสดงผลอยู่ดี

---

## การใช้ `if else` เบื้องต้น

```csharp
if (condition) 
{

} 
else 
{

}
```

+++

## ตัวอย่างที่ 1

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

 #### ผลลัพธ์

```csharp
107
```

+++

## ตัวอย่างที่ 2

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

#### ผลลัพธ์

```csharp
Oh, I'm looking for you John!
```
