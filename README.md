using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Trade_Comissions
{
    class Program
    {
        static void Main(string[] args)
        {
            string city = Console.ReadLine().ToLower();

            double sales = double.Parse(Console.ReadLine());

            if (city == "sofia")
            {
                if (sales >= 0 && sales <= 500)
                {
                    sales = sales * 5 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 500 && sales <= 1000)
                {
                    sales = sales * 7 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 1000 && sales <= 10000)
                {
                    sales = sales * 8 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 10000)
                {
                    sales = sales * 12 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else
                {
                    Console.WriteLine("error");
                }
            }
            else if (city == "varna")
            {
                if (sales >= 0 && sales <= 500)
                {
                    sales = sales * 4.5 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 500 && sales <= 1000)
                {
                    sales = sales * 7.5 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 1000 && sales <= 10000)
                {
                    sales = sales * 10 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 10000)
                {
                    sales = sales * 13 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else
                {
                    Console.WriteLine("error");
                }
            }
            else if (city == "plovdiv")
            {
                if (sales >= 0 && sales <= 500)
                {
                    sales = sales * 5.5 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 500 && sales <= 1000)
                {
                    sales = sales * 8 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 1000 && sales <= 10000)
                {
                    sales = sales * 12 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else if (sales > 10000)
                {
                    sales = sales * 14.5 / 100;
                    Console.WriteLine("{0:f2}", sales);
                }
                else
                {
                    Console.WriteLine("error");
                }
            }
            else
            {
                Console.WriteLine("error");
            }
        }
    }
}
