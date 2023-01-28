# Bonus-1
using System;
using System.Linq;

class Program
{
    static void Main()
    {
        Console.WriteLine("Enter a list of integers separated by commas: ");
        string input = Console.ReadLine();
        int[] numbers = input.Split(',').Select(int.Parse).ToArray();
        if (numbers.Length == 0)
        {
            Console.WriteLine("Error: Empty input.");
            return;
        }
        int sum = numbers.Sum();
        double average = numbers.Average();
        Console.WriteLine("Sum: " + sum);
        Console.WriteLine("Average: " + average);
    }
}
