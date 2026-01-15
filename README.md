using System

namespace Task3
{
    class Program
    {
        static void Main(string[] args)
        {
            // Declare and initialize the array
            int[] numbers = { 3, 7, 12, 19, 21, 25, 30 };

            // Ask the user for input
            Console.Write("Enter a number to search for: ");
            int searchNumber = int.Parse(Console.ReadLine());

            bool found = false;

            // Use a for loop to search the array
            for (int i = 0; i < numbers.Length; i++)
            {
                if (numbers[i] == searchNumber)
                {
                    Console.WriteLine($"Number found at position {i}!");
                    found = true;
                    break; // Stop searching immediately
                }
            }

            // If the number was not found
            if (!found)
            {
                Console.WriteLine("Number not found in the list.");
            }

            Console.ReadLine(); // Keep console open
        }
    }
}
