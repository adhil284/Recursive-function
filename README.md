# <p align="center">Recursive-function</p>

## Aim: 
To write a C# program to reverse a number using recursive function.

## Algorithm:
### Step 1:
Create a function for reversing.
### Step 2:
Get the number from the user.
### Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.
### Step 4:
Recusively call this function to get the reversed number.
### Step 5:
print the reversed number.
<br/><br/><br/><br/><br/><br/><br/><br/><br/>

## Program:
```c#
using System;
namespace Recursive
{
    class Program
    {
        public static int m, reverse = 0;
        public static int R(int n)
        {

            if (n > 0)
            {
                m = n % 10;
                reverse = reverse * 10 + m;
                n /= 10;
                return R(n);
            }
            return reverse;

        }
        static void Main(string[] args)
        {
            int num;
            Console.WriteLine("Enter a number:");
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Reverseof the number:");
            Console.WriteLine(R(num));
        }
    }
}
```

## Output:
![Capture](https://user-images.githubusercontent.com/75235747/171272049-9bb48bf9-97a2-4d81-8184-e037769218f3.JPG)
## Result:
Thus the C# program to reverse a number using recursive function is executed successfully.
