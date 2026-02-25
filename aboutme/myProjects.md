# Project One: COFFEE RUN: My First Game #
-   I created my first game, called ``COFFEE RUN``. It's an arcade style game. The goal is to collect all the coffee ingredients and get them to the machine to brew a coffee before getting killed by enemies! 
-   This console game was created using ``Visual Studio 2022``, coded in ``C#``.

## Code Snippet: ##
-   The following code snippet is the menu portion of my code!

    static void Menu()
        {
            bool running = true;

            while (running)
            {
                Console.Clear();
                Console.ForegroundColor = ConsoleColor.Magenta;
                WriteCentered("╔════════════════════════════════╗");
                WriteCentered("║   Welcome to COFFEE RUN!!!     ║");
                WriteCentered("╚════════════════════════════════╝");
                Console.WriteLine();
                WriteCentered(" Press 1 to PLAY");
                WriteCentered(" Press 2 for INSTRUCTIONS");
                WriteCentered(" Press 3 to QUIT");
                WriteCentered("Please enter your choice: ");

                string input = Console.ReadLine();
                if (!int.TryParse(input, out int choice))
                {
                    WriteCentered("Invalid input. Press any key to continue...");
                    Console.ReadKey(true);
                    continue;
                }

## Screenshots ##



## What I learned ##
> I learned a lot about how to validate user input for more than just selecting menus. I learned how to make character move. Assigning keys to keystroke, using Console.key etc...






# Project Two: Console Math Mini Games
-   This was one of my first coding projects. The goal was to learn how to create a menu navigation system using switch cases, and to validate user input by using Console.Readline().
-   It features 5 different math style games. ``"Area of Rectangles"``, ``"Collatz Conjecture"``, ``"Dollar Game"``, ``"Oldest Person"`` and ``"Hi Lo Game"``.

## Code Snippet: ##
-    The following is a code snippet for the first switch case which contains the ``Area of Rectangle`` game.
Int32 choice;
            choice = Convert.ToInt32(Console.ReadLine());
                switch (choice)
                {
                    case 1: // GAME 2: AREA OF RECTANGLES START
                        Console.Clear();
                        Console.WriteLine(" Area of Rectangles ");

                        Console.WriteLine(" Welcome to AREA OF RECTANGLES!");
                        Console.WriteLine(" In this game, I will tell you which rectangle is bigge depending on the length/width of each.");
                        Console.WriteLine(" Please enter a whole number to represent the LENGTH of the FIRST rectangle.");
                        int length1 = Convert.ToInt32(Console.ReadLine()); // CALL FOR USER INPUT
                        Console.WriteLine(" Please enter a whole number to represent the WIDTH of the FIRST rectangle");
                        int width1 = Convert.ToInt32(Console.ReadLine()); // CALL FOR USER INPUT

                        Console.WriteLine(" Now, please enter a whole number to represent the LENGTH of the SECOND rectangle");
                        ; int length2 = Convert.ToInt32(Console.ReadLine()); // CALL FOR USER INPUT
                        Console.WriteLine(" Please enter a whole number to represent the WIDTH of the SECOND rectangle");
                        int width2 = Convert.ToInt32(Console.ReadLine()); // CALL FOR USER INPUT

                        // CREATION AND DEFINITION

                        int area1 = length1 * width1;
                        int area2 = length2 * width2;

                        if (area1 == area2)
                            Console.WriteLine(" Your rectangles are the same area at " + area1 + " meters square");

                        else
                            if (area1 > area2)
                            Console.WriteLine(" The FIRST rectangle has a greater area of " + area1 + " meters square");

                        else
                            Console.WriteLine(" The SECOND rectangle has a greater area of " + area2 + "meters square");


                        Console.WriteLine();
                        Console.WriteLine(" Please press any button to go back to the menu!");
                        Console.ReadKey();

                      

                        break;

                        // NEW GAME

## Screenshots ##



## What I learned ##
>With this one, this was the moment I started becoming comfortable using switch cases. After this I have continued using this method for menu creation.
>I also worked a lot with mathematics in coding, and learnt about how math can manipulate variables.