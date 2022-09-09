# Pattern
## Aim:
To write a C# program for a pascal's triangle.
## Equipment Required:
1.Hardware-PC

2.Visual Studio Code 2022.
## Algorithm:
### Step 1:
Start.
### Step 2:
Create a class and declare two variables rows,Val using integer datatype.
### Step 3:
Using nested for loop we can create a pascal's triangle according to the value intialised.
### Step 4:
Stop.

## Program:
```
Program Developed by: S.SHAM RATHAN
Register Number: 212221230093
using System;

namespace pascal_triangle
{
    class Program
    {
        static void Main(string[] args)
        {
            int rows = 5, val = 1;
            for (int i = 0; i < rows; i++)
            {
                for (int blank = 1; blank < rows - i; blank++)
                {

                    Console.Write(" ");
                }
                for (int j = 0; j <= i; j++)
                {
                    if (i == 0 || j == 0)
                        val = 1;
                    else
                        val = val * (i - j + 1) / j;
                    Console.Write(val + " ");

                }

                Console.WriteLine();

            }

        }
    }
}
```

## Output:
![pascal](https://user-images.githubusercontent.com/93587823/189411363-08141c3f-1499-4382-97b3-408c13de208d.png)


## Result:
Thus the C# program to print the pascal's triangle is executed successfully.
