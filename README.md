# Recursive-function

## Aim: 
To write a C# program to reverse a number using recursive function.

## Algorithm:
## Step 1:
Create a function for reversing.

## Step 2:
Get the number from the user.

## Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

## Step 4:
Recusively call this function to get the reversed number.

## Step 5:
print the reversed number.
## Program:
```
using System;
namespace hello
{
    class Program
    {
        int rem = 0, rev = 0;
        public int reverse(int n)
        {
            rem = n % 10;
            if (rem == 0) return rev;
            else
            {
                rev = rev * 10 + rem;
                return reverse(n / 10);
            }
        }
        static void Main(string[] args)
        {
            int n;
            Console.WriteLine("Enter a Number to reverse: ");
            n = Convert.ToInt32(Console.ReadLine());

            Program p1 = new Program();
            Console.WriteLine("Reversed Number is "+ p1.reverse(n));
        }
    }
}
```

## Output:
![image](https://user-images.githubusercontent.com/94164665/173244936-400fcb74-d7e2-4655-980f-3e4ae51ea393.png)

## Result:
C# program to reverse a number using recursive function is executed successfully.

