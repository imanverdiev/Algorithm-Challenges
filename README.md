# Algorithm-Challenges
Question 1.
## Problem: Array Sum

### Input Format

- The first line contains an integer, `n`, denoting the size of the array.
- The second line contains `n` space-separated integers representing the array's elements.

### Output Format

- Print the sum of the array's elements as a single integer.
- 
### Solution

```csharp
using System;
using System.Linq;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Enter the size of the array:");
        int countArr = int.Parse(Console.ReadLine());

        Console.WriteLine("Enter the elements as space-separated:");
        string[] elements = Console.ReadLine().Split(' ');

        if (elements.Length != countArr)
        {
            Console.WriteLine("The number of elements does not match the specified array size.");
            return;
        }

        int sum = elements.Sum(int.Parse);
        Console.WriteLine($"The sum of the array elements is: {sum}");
    }
}

