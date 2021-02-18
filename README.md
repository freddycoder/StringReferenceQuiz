# StringReferenceQuiz
Quiz to test your uderstanding of c# string instance.

# Extract from Program.cs

```
        const string BonjourLeMonde = "Bonjour le monde!";

        static string HolaMundo()
        {
            return "Hola mundo";
        }

        static void Main(string[] args)
        {
            // Try to guess what is going to be print in the console.

            string a = "Hello world!";
            string b = "Hello world!";

            string c = BonjourLeMonde;

            string d = "Hola mundo";

            if (ReferenceEquals(a, b))
            {
                Console.WriteLine(a);
            }

            if (ReferenceEquals(c, BonjourLeMonde))
            {
                Console.WriteLine(BonjourLeMonde);
            }

            if (ReferenceEquals(HolaMundo(), d))
            {
                Console.WriteLine(HolaMundo());
            }

            string reflectedString = nameof(reflectedString);

            if (ReferenceEquals("reflectedString", reflectedString))
            {
                Console.WriteLine(reflectedString);
            }

            var @string = typeof(string).Name;
            var sa = "string";

            if (Equals(@string, sa))
            {
                Console.WriteLine("Equals " + sa);
            }

            if (ReferenceEquals(@string, sa))
            {
                Console.WriteLine("ReferenceEquals " + sa);
            }

            var sb = "String";

            if (Equals(@string, sb))
            {
                Console.WriteLine("Equals " + sb);
            }

            if (ReferenceEquals(@string, sb))
            {
                Console.WriteLine("ReferenceEquals " + sb);
            }
        }
```

Compile the program to get the answer. Good luck!
