# Order ID Fraud Detection

This project contains a simple C# program that helps in detecting potential fraudulent orders. Our team has found a pattern where orders that start with the letter "B" encounter fraud at a rate 25 times greater than the normal rate. To aid in the investigation of such cases, we have developed a program that outputs the Order ID of new orders where the Order ID starts with the letter "B".

## Code Overview

The code is written in C# and it uses a simple `foreach` loop to iterate over an array of order IDs. For each order ID, it checks if the ID starts with the letter "B". If it does, the order ID is printed to the console. This output can then be used by the fraud team for further investigation.

Here is the main code:

```csharp
string[] orders = {"B123", "C234", "A345", "C15", "B177", "G3003", "C235", "B179"};

foreach (string order in orders)
{
    if (order.StartsWith("B"))
    {
        Console.WriteLine(order);
    }
}
