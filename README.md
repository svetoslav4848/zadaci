# zadaci



using System;

namespace test_zadacha6
{
    class Program
    {
        static void Main(string[] args)
        {
            int mens = int.Parse(Console.ReadLine());
            int womens = int.Parse(Console.ReadLine());
            int tables = int.Parse(Console.ReadLine());
            int reservedTables = 0;
            for (int i = 1; i <= mens; i++)
            {
                for (int j = 1; j <= womens; j++)
                {
                    reservedTables++;
                    if (reservedTables <= tables)
                    {
                        Console.Write("({0} <-> {1}) ", i, j);
                    }
                }
            }
        }
    }
}
