using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {
            int b = 150;
            string answer;
            Console.WriteLine("Тебе нравятся девушки?");
            answer = Console.ReadLine();
            if (answer == "нет")
                Console.WriteLine("Ну ок, тогда нам не о чем говорить");
            else if (answer == "да")
            {
                Console.WriteLine("Высокие или низкие?");
                answer = Console.ReadLine();
                if (answer == "высокие")
                {
                    Console.WriteLine("А какой твой рост?");
                    int c = Convert.ToInt32(Console.ReadLine());
                    if (c < b)
                        Console.WriteLine("ахаха)");
                    else if (c > b)
                        Console.WriteLine("Спасибо за ваш отзыв!");
                }
                else if (answer == "низкие")
                {
                    Console.WriteLine("А какой твой рост?");
                    int d = Convert.ToInt32(Console.ReadLine());
                    if (d < b)
                        Console.WriteLine("Спасибо за Ваш отзыв!");
                    else if (d > b)
                        Console.WriteLine("Ахаха))");
                }
            }
            Console.ReadLine();
        }
    }
}
