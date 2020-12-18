# CF_431A_Black_square
	using System;

namespace string_generation
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] arr = new int[5];
            string[] t = (Console.ReadLine()).Split(' ');
            for(int i=1;i<=4;i++)
            {
                arr[i] = int.Parse(t[i-1]);
            }
            string str = Console.ReadLine();
            long sum = 0;
            for(int i=0;i<str.Length;i++)
            {
                sum += arr[Convert.ToInt32(str[i])-'0'];
            }
            Console.WriteLine(sum);

        }
    }
}
