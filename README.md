# Test1
  static void Main(string[] args)
        {
            Random rnd = new Random();
            int num = rnd.Next(0, 100);
            int guess;
            int count = 0;

            do
            {
                Console.WriteLine("Try guessing the number between 1-100");
                guess = int.Parse(Console.ReadLine());
                if (guess == num)
                {
                    Console.WriteLine("hurrah you won with only "+count+" attempts");
                    count++;
                }
                else if (guess < num)
                {
                    Console.WriteLine("try little higher");
                    count++;
                }
                else
                {
                    Console.WriteLine("try little lower");
                    count++;
                }
            } while (guess != num);     
                
