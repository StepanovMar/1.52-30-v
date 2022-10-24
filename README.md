using System;

namespace ConsoleApp6
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Цена 1 кг конфет - 13р. Введите кг: ");
            double sweets = double.Parse(Console.ReadLine());

            Console.Write("Цена 1 кг печенья - 11р. Введите кг: ");
            double biscuits = double.Parse(Console.ReadLine());

            Console.Write("Цена 1 кг яблок - 7р. Введите кг: ");
            double apples = double.Parse(Console.ReadLine());

            double stoimostSweets = sweets * 13;
            double stoimostBiscuits = biscuits * 11;
            double stoimostApples = apples * 7;
            Console.WriteLine($"Стоимость конфет: {stoimostSweets} руб");
            Console.WriteLine($"Стоимость печенья: {stoimostBiscuits} руб");
            Console.WriteLine($"Стоимость яблок: {stoimostApples} руб");

            double sumaStoimost = stoimostSweets + stoimostBiscuits + stoimostApples;
            Console.WriteLine($"Общая стоимость покупки: {sumaStoimost} руб");

            Console.ReadLine();
        }
    }
}
