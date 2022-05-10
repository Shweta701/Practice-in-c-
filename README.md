# Practice-in-c-

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp31
{
    class Program
    {
        static void Main(string[] args)
        {

            //Cheak the Number is Prime or Not


            int count = 0;
            Console.WriteLine("Enter the Number to Cheak the Number is Prime Or Not:");
            int n = int.Parse(Console.ReadLine());
            for (int i = 1; i <= n; i++)
            {
                if (n % i == 0)
                {
                    count++;
                }
            }
            if (count == 2)
            {
                Console.WriteLine("Number is Prime.");
            }
            else
            {
                Console.WriteLine("Number is not Prime.");
            }

            //Cheak the Number is Palindrome or not.

            int rem;
            int res = 0;
            int temp;
            Console.WriteLine("Enter the Number to Cheak the Number is Palindrome or Not:");
            int n = int.Parse(Console.ReadLine());
            temp = n;
            while (n != 0)
            {
                rem = n % 10;
                res = res * 10 + rem;
                n = n / 10;
            }
            if (temp == res)
            {
                Console.WriteLine("The Number is Palindrome.");
            }
            else
            {
                Console.WriteLine("The Number is Not Palindrome.");
            }

            //Print Fibbonaci Series.
            int a = 0;
            int b = 1;
            Console.WriteLine(a);
            Console.WriteLine(b);
            for (int i = 0; i <= 10; i++)
            {
                int c = a + b;
                Console.WriteLine(c);
                a = b;
                b = c;
            }

            //Cheak the Number is Armstrong or not.

            int rem;
            int res = 0;
            int cube;
            int temp;
            Console.WriteLine("Enter the Number to Cheak the Number is Armstrong or not:");
            int n = int.Parse(Console.ReadLine());
            temp = n;
            while (n != 0)
            {
                rem = n % 10;
                cube = rem * rem * rem;
                res = res + cube;
                n = n / 10;
            }
            if (temp == res)
            {
                Console.WriteLine("Number is Armstorng.");
            }
            else
            {
                Console.WriteLine("Number is not Armstrong.");
            }
            Console.ReadLine();
        }
    }
}
