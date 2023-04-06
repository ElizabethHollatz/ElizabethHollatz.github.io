## Portfolio

---

### PROG101 

[Devour](/sample_page)
<"internal class Game
    {
        private Player player;
        string GameTitle = "Devour";

        public Game()
        {
            player = new Player();
        }




        public void Grocer()
        {
            
                WriteLine("The bell still chimes when you open the grimey glass door. " +
                "\n The shelves are still just as barren as they were a year ago. " +
                "\nEmergency supplies haven't been here in the past 16 months. " +
                "\nI think the government forgot about Violet Lake.");
                ReadKey();
                Clear();
                WriteLine("Eh, needs em? I get by plenty well on my own." +
                    "\n You look around for any more supplies you might have missed, and come across a bag of frozen strawberries tucked in the corner of the freezer." +
                    "\n +1 food");
                player.AddInventory("Food");
                ReadKey();
                WriteLine("Would you like to?" +
                    "1. Go home?" +
                    "OR" +
                    "2. Go back to main street");
                string answer = ReadLine();
                //does not let player input choice
                //add option to go back to main or go home
                //in class conditional statements
                if (answer == "1")
                {
                // go to home
                Home();
                }
                else if (answer == "2")
                {
                    // go back to main street
                    MainStreet();
                }
                else
                {
                    WriteLine("Uh, Not sure what you mean by that. Enter 1 or 2 to pick a location.");
                }
            
        }




        public void MainStreet()
        {
            WriteLine(
           "You stare down the dusty road and smell the pine trees. Out in the distance is the lake." +
           "\n Where will you go?" +
           "\n 1. The Grocer?" +
           "\n 2. The Taco truck?" +
           "\n 3. The Lake?" +
           "\n 4. The Pharmacy?");
            string input = ReadLine();
            Clear();
            if (input == "1")
            {
                Clear();
                Grocer();
            }


            else if (input == "2") //w3 schools else if
            {
                Clear();
                TacoTruck();


            }


            else if (input == "3")
            {
                Clear();
                Lake();

            }


            else if (input == "4")
            {
                Clear();
                Pharmacy();


            }

            //make this not show up >:)
            else
            {
                WriteLine("Uh, not sure what you mean by that. Type a number 1-4 to pick a location");
                MainStreet();
            }
        }





        public void Home()
        {
            Clear();
            WriteLine("You walk up the gravel road that has your house at the end of it. It still looks the same as when this whole mess started.");
            ReadKey();
            WriteLine("It looks like shit.");
            ReadKey();
            WriteLine("You and your dad never really had a thing for 'home metience' or 'Curb appeal'. HGTV would have loved to flip this house.");
            ReadKey();
            WriteLine("Good thing they're all dead, I guess.");
            ReadKey();
            Clear();
            WriteLine("This has been your home for as long as you remember. You still get those damned warm and fuzzy feelings walking up to the large porch, remembering all the bikes, scooters, and sport equipment that scrateched the paint off of the wood.");
            ReadKey();
            WriteLine("Your mom used to get SOOO mad at you for that.");
            ReadKey();
            WriteLine("... Well anyways.");
            Clear();
            WriteLine("You open the front door and head to the living room, flopping down on the couch. \n You check for scrapes and gashes and patch up what you can with what you have.");
            ReadKey();
            WriteLine("You hear a soft scratching sound from the door. You're immedietly alarmed and get up to see what is making that noise.");
            ReadKey();
            WriteLine("mrrreow?");
            ReadKey();
            WriteLine("Do you? \n1. Open the door." +
                "OR" +
                "2. Go back to what you were doing?");
            string input2 = ReadLine();
            if (input2 == "1")
            {
                Clear();
                Console.WriteLine(" You crack the door open and see a beautiful orange kitty with green eyes looking up at you.");
                ReadKey();
                WriteLine("Do you?" +
                    "1. Let the cat in" +
                    "OR" +
                    "2. Close the door");
                string input3 = ReadLine();
                if (input3 == "1") 
                {
                    Clear();
                    WriteLine("You swing the door open and the cat trotts his way inside and lays down on the couch. \n You smile.");
                    ReadKey();
                    WriteLine("You walk over to the cat and bring your hand down to pet the cat and...");
                    if (player.Inventory.Contains("Food"))
                    {
                        WriteLine("The cat smells the food you collected today and happily snuggles in. You notice this, and share some of your dinner with the cat.");
                        ReadKey();
                        Clear();
                        WriteLine("CONGRATULATIONS!! YOU HAVE ADOPTED A CAT!");
                        ReadKey();
                        WriteLine("You live out the rest of the apolcolypse with your little warrior. You live a happy life, and feel as if you are never lonely.");
                        ReadKey();
                        WriteLine("THE END");
                    }
                    else if (player.Inventory.Contains("Rainbow Trout"))
                    {
                        WriteLine("The cat smells the rainbow trout you collected today and happily snuggles in. You notice this, and share some of your dinner with the cat.");
                        ReadKey();
                        WriteLine("The cat was so happy with his meal he invited his cat freinds to join him. The arrived in the morning, and spent breakfast with you. \n After a little grooming, they are all so soft and cuddly. You haven't been this happy in a long time. \n Thye hunt for mice themselves, and can sustain themselves a little on their own, but with your new found talent in fishing, everyone eats well.\n you are happy.");
                        Clear();
                        WriteLine("CONGRATULATIONS!! YOU HAVE ADOPTED A CAT! \nBonus! Cat Colony award!");
                        ReadKey();
                        WriteLine("You live out the rest of the apolcolypse with your little warriors. You live a happy life, and feel as if you are never lonely.");
                        ReadKey();
                        WriteLine("THE END :3");

                    }
                    else
                    {
                        Clear();
                        WriteLine("The cat's stomach grumbles, and he leaps out off the couch, and slips out of the door. As if it *Magically Knew* That you had no food on you!");
                        ReadKey();
                        WriteLine("Wow, videogame magic.");
                        ReadKey();
                        Clear();
                        WriteLine("You live off the land for the rest of your life, crafting a green house and collecting some barn animals.");
                        ReadKey();
                        WriteLine("However, they never really fill the hole that adorbale cat left in your heart, and you die alone.");
                        ReadKey();
                        Clear();
                        WriteLine("YOU WON?");
                    }

                }
                else if (input3 == "2")
                {
                    Clear();
                    WriteLine("You shut the door into the cat's face.");
                    ReadKey();
                    WriteLine("You monster.");
                    ReadKey();
                    WriteLine("You live off the land for the rest of your life, crafting a green house and collecting some barn animals.");
                    ReadKey();
                    WriteLine("However, they never really fill the hole that adorbale cat left in your heart, and you die alone.");
                    ReadKey();
                    Clear();
                    WriteLine("YOU WON?");
                }
                else
                {
                    Console.WriteLine("How the hell did you get so far in this game?? This was literally the last option (SPOILERS!), how did you mess it up NOW? Enter 1 or 2 to pick an option");
                }
            }
            else if (input2 == "2")
            {
                Clear();
                WriteLine("'Meh, they'll go away on their own.'You say to yourself as you continue to clean your wounds.");
                ReadKey();
                WriteLine("You live off the land for the rest of your life, crafting a green house and collecting some barn animals.");
                ReadKey();
                WriteLine("However, they never really fill a specific hole in your heart, and you die alone.");
                ReadKey();
                Clear();
                WriteLine("YOU WON?");
            }
            else
            {
                Console.WriteLine("Uh, not sure what you mean by that. Enter 13 or 14 to pick an option");
            }
        }




        public void TacoTruck()
        {
            WriteLine("The red truck's paint has dulled under the sun," +
                "\n and it looks like the world forgot about this local favorite." +
                "\n You swing open the rusty door, hoping to find any scraps of food, or even a med pack or fire extinguisher.");
            ReadKey();
            Clear();
            WriteLine("Unfortunatly, you didnt expect to find a dozen raccoons making their home atop the grill and in the open oven.");
            ReadKey();
            WriteLine("Their eyes snap to yours and start to charge at you. \n Do You? \n 1.Grab your weapon and fight? \n OR \n 2. Run!");
            //does not let player insert answer
            string choice = ReadLine();
            if (choice == "1")
            {
                Clear();
                WriteLine("...");
                ReadKey();
                WriteLine("...");
                ReadKey();
                WriteLine("You tried your best to fight, but the raccoons are close friends and use the power of frienship to beat your ass");
                ReadKey();
                Clear();
                WriteLine("YOU DIED");
                ReadKey();
                
            }
            else if (choice == "2")
            {
                WriteLine("You run as fast as you legs will take you. You arent sure where you are heading, until...");
                Home();
            }
            else
            {
                Console.WriteLine("Uh, not usre what you mean by that, enter 1 or 2 to pick an option.");
                TacoTruck();
            }
        }

        public void Lake()
        {
            Console.WriteLine("The sun glisens over the water, causing the deep blue water to sparkle like the stars." +
                "\n The dark pine trees loom overhead all around the lake, appreciating the rare sun rays. " +
                "\nWith how wild the nature has gotten, it's impossible to imagine that this used to be a touristy town.");
            Console.ReadKey();
            Console.WriteLine("Man, I havent tried fishing in ages." +
                "\n You search the beach for a net or fishing rod.");
            Console.ReadKey();
            //microsoft
            Random random = new Random();
            int NetNumber = random.Next(1, 3);

            Console.WriteLine("Pick a number between 1-2");
            string guessInput1 = Console.ReadLine();
            int number = int.Parse(guessInput1);

            int guess;
            if (int.Parse(guessInput1) == NetNumber)
            {
                Console.WriteLine("You find a large scrap of netting usually used for plastic fencing in construction areas." +
                    "\n It might work.");
                Console.ReadKey();
                Console.Clear();
                FishingGame();
            }
            else
            {
                Console.WriteLine("Aw, you don't see anything, and begin to walk home.");
                Console.ReadKey();
                Console.Clear();
                Home();
            }





        }
        public void FishingGame()
        {
            //microsoft
            Random random = new Random();
            int fishNumber = random.Next(1, 6);

            Console.WriteLine("Pick a number between 1-5");
            string guessInput = Console.ReadLine();
            int number = int.Parse(guessInput);

            int guess;
            if (int.Parse(guessInput) == fishNumber)
            {
                Console.WriteLine("CONGRATS! YOU CAUGHT A RAINBOW TROUT! \n+1 food");
                player.AddInventory("Rainbow Trout");
                WriteLine("Would you like to go home?" +
                    "1. Yes" +
                    "2. No, Back to main street.");
                string choice11 = ReadLine();
                if (choice11 == "1")
                {

                    Home();
                }
                else if (choice11 == "2")
                {

                    MainStreet();
                }
                else
                {
                    Console.WriteLine("Uh, not sure what you mane by that. Pick either 1 or 2 to choose a location.");

                    Lake();
                }

            }
            else
            {
                Console.WriteLine("Shit. You didnt catch anything.");
                Console.ReadLine();
                WriteLine("Try again?\n1. Yes \n2. No");
                string choice999 = ReadLine();
                if (choice999 == "1")
                {
                    FishingGame();
                }
                else if (choice999 == "2")
                {
                    MethodFishingGiveUp();
                    
                }
                
                

                
            }
        }
        public void MethodFishingGiveUp()
        {
            WriteLine("1.Go Home\n2.Go back to main street.");
            string FishingGiveUp = ReadLine();
            if (FishingGiveUp == "1")
            {
                Console.WriteLine("I'm tired, I gotta head home and get something to eat.");
                Console.ReadLine();
                Home();
            }
            else if (FishingGiveUp == "2")
            {
                MainStreet();
            }
            else
            {
                Console.WriteLine("Uh, dont know what you mean by that. Enter 1 or 2 to pick a location.");
                MethodFishingGiveUp();
            }
        }


        public void Pharmacy()
        {
            Console.WriteLine("When you walk inside you feel the stink of alcohol waft over your face.");
            Console.ReadKey();
            Console.WriteLine("'Who the fuck is that?' A voice calls from behind the prescription counter." +
                "\n You instinctivly grasp the gun on your hip after hearing a voice." +
                "\n Do you?" +
                "\n 1. Investigate the voice?" +
                "\n 2. Go Home");
            //does not let player enter answer
            string input1 = ReadLine();

            if (input1 == "1")
            {

                if (player.Inventory.Contains("Rainbow Trout"))
                {
                    Clear();
                    WriteLine("'I SAID, WHO THE FUCK IS THAT' The voice yells even louder. They sound hungry");
                    ReadKey();
                    WriteLine("'Just someone passing through, looking for some bandages.' You say, making your way through the store. \n 'Well, youre gonna need more then bandages after meeting me.'");
                    ReadKey();
                    WriteLine("'Is that a fucking threat?' You yell, starting to work yourself up for a fight.");
                    ReadKey();
                    Console.WriteLine("You pass into the perscription area, and start looking between the shelves, looking for the source of that voice. You hear a deep inhale come from behind you.");
                    ReadKey();
                    WriteLine("'Well, this looks like a tasty meal...' You turn around and all you see is a big silly guy with a shotgun axe, sniffing the air. \nYou pull out the Rainbow Trout that has been stinking up your bag and hold it out to him. \n'Looking for this?'");
                    ReadKey();
                    WriteLine("'OooOOOoooOOOOoooOOOooh Yeahhh!!!' He starts jumping up and down, and grabs the fish from you and starts chomping down. You laugh.");
                    ReadKey();
                    WriteLine("CONGRATULATIONS!. \nYou found the secret ending! \nYou lived off the rest of your life with Gerald, a life on the lake full of tasty fish and good conversation. You almost never feel alone. \nThe End!");
                }
                else
                {
                    Clear();
                    WriteLine("'I SAID, WHO THE FUCK IS THAT' The voice yells even louder. They sound hungry");
                    ReadKey();
                    WriteLine("'Just someone passing through, looking for some bandages.' You say, making your way through the store. \n 'Well, youre gonna need more then bandages after meeting me.'");
                    ReadKey();
                    WriteLine("'Is that a fucking threat?' You yell, starting to work yourself up for a fight.");
                    ReadKey();
                    Console.WriteLine("You pass into the perscription area, and start looking between the shelves, looking for the source of that voice. You hear a deep inhale come from behind you.");
                    ReadKey();
                    WriteLine("'Well, this looks like a tasty meal...' You turn around and all you see is a shotgun axe coming down on your face.");
                    ReadKey();
                    WriteLine("YOU DIED. \nYou got eaten by Gerald!");
                }

                //add something to restart the game

            }
            else if (input1 == "2")
            {

                Home();
            }
            else
            {
                Console.WriteLine("Uh, not sure what you mean by that. Enter 1 or 2 to pick an option");
                Console.ReadKey();
                Pharmacy();
            }
        }


        

    




        public void Start()
        {
            

            WriteLine("It's been 5 fucking years since I've had a coffee in this coffee shop.");
            ReadKey();
            WriteLine("And no, its not becuase the service here sucked. \n(Although, that was definetly true. The teenagers from Charger's high were real assholes.)");
            ReadKey();
            Clear();
            WriteLine("This sleepy town got a whole lot sleepier after the zombie plauge unleached it's wrath on the world.");
            ReadKey();
            WriteLine("I'm not sure if anyone else is left \nExcept me.");
            ReadKey();



            WriteLine("I'm not sure if I have a name anymore.");
            ReadKey();
            WriteLine("What is your name?");
            player.Name = ReadLine();
            WriteLine(player.Name + ". " + player.Name + ". " + player.Name + ".\n God, I got to get out of my head.");
            ReadKey();
            Clear();


            WriteLine("You stand up and leave the mug n slice. " +
            "\n You stare down the dusty road and smell the pine trees. Out in the distance is the lake." +
            "\n Where will you go?" +
            "\n 1. The Grocer?" +
            "\n 2. The Taco truck?" +
            "\n 3. The Lake?" +
            "\n 4. The Pharmacy?");
            string input = ReadLine();
            



            if (input == "1")
            {
                Clear();
                Grocer();
            }


           else if (input == "2")
            {
                Clear();
                TacoTruck();


            }


           else if (input == "3")
            {
                Clear();
                Lake();

            }


           else if (input == "4")
            {
                Clear();
                Pharmacy();


            }

            //make this not show up >:)
            else
            { WriteLine("Uh, not sure what you mean by that. Type a number 1-4 to pick a location");
                MainStreet();
            } 
                        
                     


        } 
        

         

}

    }
    
    internal class Player
    {
        public string Name;
        public List<string> Inventory { get; set; }
        public Player() 
        {
            Inventory = new List <string>();
        }
        //microsoft
        public void AddInventory(string item)
        {
            Inventory.Add(item);
        }
        //microsoft
        public void PrintInventory()
        {
            Console.WriteLine("Inventory");
            foreach (string item in Inventory)
            {
                Console.WriteLine(item);
            }

        }
        

    }
    
   internal class Gerald
    {
        public List<string> Inventory { get; set; }
        //microsoft
        public Gerald()
        {
            Inventory = new List<string>();
        }
        public string Name { get; set; }
        public Gerald(string name)
        {

            this.Name = name;

        }

        Gerald nameGerald = new Gerald("Gerald");


    }
  internal class FishingNet
    {
        public int durability { get; set; }
        public FishingNet(int durability)
        {

            this.durability = durability;

        }

        FishingNet fishingnetdurability = new FishingNet(10);
        

    }
  public string Breed { get; set; }
        //microsoft
        public Fish(string breed)
        {

            this.Breed = breed;

        }

        Fish FishBreed = new Fish("Rainbow Trout");

    }
  internal class Cat

    {
        //Microsoft
        public string Name { get; set; }
        public Cat(string name)
        {

            this.Name = name;
            
        }

        Cat cuteCat = new Cat("Obi");
        
        

    }
   internal class Program
    {
        static void Main(string[] args)
        {
            Game game = new Game();
            game.Start();
        }


    }
  ">

---
[Puppet History Quiz Show](/pdf/sample_presentation.pdf)
<" internal class Game
    {//Beth Hollatz 2023
        private Player player1;
        private List<TriviaItem> trivia = new List<TriviaItem>();

        public Game() 
        {
            //TODO start my game
            GreetPlayer();
            LoadQuiz();
            Quiz();
        }

        public void GreetPlayer()
        { 
         WriteLine("Welcome one and all to the Puppet History Quiz Show! \nSeason 5! \nI'm assuming you know all about Puppet history (and Watcher) if you found this quiz, So I expect an amazing score!\n(unless you are my programming professor, hello! This will be confusing for you.)\n\nWhat is your name?");
            player1 = new Player(ReadLine());
            //Test input of player name
            //WriteLine(player1.Name);
        }
        //list
        public void LoadQuiz()
        {
            TriviaItem item1 = new TriviaItem("Who is beef boy?", "Ryan Bergara");
            TriviaItem item2 = new TriviaItem("Who replaced the professor after his tragic death (via beef boys hands)?", "The substitute");
            TriviaItem item3 = new TriviaItem("What hot daga character was visible behind the curtain in one episode?", "Gene, who is french fries");
            TriviaItem item4 = new TriviaItem("What did the cloud witness while looking down at the world one day?", "The JFK Assasination");
            TriviaItem item5 = new TriviaItem("What happened to beef boy while fighting the infinitiger ?", "His arm got bitten off");
            TriviaItem item6 = new TriviaItem("What name did the substute order the genie lamp under?", "Concupisence McNasty");
            TriviaItem item7 = new TriviaItem("Who got defenestrated out the example window?", "The substitute");

            trivia.Add(item1);
            trivia.Add(item2);
            trivia.Add(item3);
            trivia.Add(item4);
            trivia.Add(item5);
            trivia.Add(item6);
            trivia.Add(item7);

        }

        public void Quiz()
        {// printing one item at a time
            //WriteLine(trivia[0].ShowQuestion());

            //use a loop to iterate through all items at once
            //print question
            //take input
            //print answers

            for (int i = 0; i < trivia.Count; i++)
            {
                WriteLine(trivia[i].ShowQuestion());
                var response = ReadLine();
                WriteLine($"The correct answer is {trivia[i].GetAnswer()}, You entered {response}");
                Clear();
            }

        }

    }">

---
[Adopt A Robot](http://example.com/)
<"internal class Game
    {
        Player player;
        string GameTitle = "Adopt a bot!";

        public Game()
        {
            player = new Player();
        }
        public Game(string title)
        {
            GameTitle = title;
            player = new Player();

        }

        public object GreetPlayer { get; private set; }

        public object SayHello { get; private set; }

        public object AdoptBot { get; private set; }

        public object PickColor { get; private set; }

        public object ColorChoice { get; private set; }
      
        public object CongratulatePlayer { get; private set; }

        public void Start()
            
        {
            System.Console.Title = GameTitle;
            object greetPlayer = GreetPlayer;
            {
                System.Console.WriteLine("Welcome to the Robot Adoption Center!");
                System.Console.WriteLine("What is your name?");
                player.Name = System.Console.ReadLine();

            }


            object sayHello = SayHello;
            {
                System.Console.WriteLine("Nice to meet you " + player.Name);

            }


            object adoptBot = AdoptBot;
            {
                System.Console.WriteLine($"Ready to adopt a bot?");

                System.Console.WriteLine("What should their name be?");
                player.PlayerRobot.Name = System.Console.ReadLine();

            }


            object pickColor = PickColor;
            {
                System.Console.WriteLine("Type a number to pick a color for your new robot! 1) Red 2) Blue 3) Purple 4) Yellow 5) Black 6) Green");
                string choice = System.Console.ReadLine();



                object colorChoice = ColorChoice;
                switch (choice)
                {
                    case "1":
                        player.PlayerRobot.Color = "Red";
                        break;
                    case "2":
                        player.PlayerRobot.Color = "Blue";
                        break;
                    case "3":
                        player.PlayerRobot.Color = "Purple";
                        break;
                    case "4":
                        player.PlayerRobot.Color = "Yellow";
                        break;
                    case "5":
                        player.PlayerRobot.Color = "Black";
                        break;
                    case "6":
                        player.PlayerRobot.Color = "Green";
                        break;
                }

            }


            object congratulatePlayer = CongratulatePlayer;
            {
                System.Console.Clear();
                System.Console.WriteLine($"YIPPEE {player.Name}!! You have adopted a {player.PlayerRobot.Color} robot named {player.PlayerRobot.Name}. Press any key to exit.");
                System.Console.ReadKey();

            }
           
            
        }
    }
         class Player
    {
        public string Name;
        public Robot PlayerRobot;

        public Player() 
        {
            PlayerRobot = new Robot("Robot Mach II", "Silver");
        
        }

    }
         internal class Robot
    {
        public string Name;
        public string Color;
        public Robot(string name, string color)
        {
            Name = name;
            Color = color;
        }
    }
         static void Main(string[] args)
        {
            Game game = new Game("Adopt a Robot Game!");
            game.Start();
        }"   >

---


---




---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
