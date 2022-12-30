using System;

public class HelloWorld
{
    public static void Main(string[] args)
    {
   
     
       Console.WriteLine("start number");
         int num1=int.Parse(Console.ReadLine());
         Console.WriteLine("end number");
         int num2=int.Parse(Console.ReadLine());
         
        for (int i =num1; i <= num2; i++)
        {
            int sum = 0;
            for (int j = 1; j < i; j++) 
            {
                if (i%j == 0) 
                {
                    sum += j;
                }
            }
            if (sum == i) 
            {
                Console.WriteLine("'{0}' is Perfect",i);
            }

        }

    }
}