# a text-based adventure game set in a hospital

import time

# values: (keys)-> direction, (value)-> room
rooms = {
    "White_Room": {
        "Door": "Corridor",
        "or Inspect": "Description"
    },
    "Corridor": {
        "Left": "Bathroom",
        "or Right": "Cafeteria"
    },
    "Bathroom": {
        "Investigate": "Red or Blue",
        "or Back": "Corridor"
    },
    "Cafeteria": {
        "Right": "Staircase",
        "or Left": "Corridor"
    },
    "Staircase": {
        "Back to Cafeteria (Type 'Back')": "Cafeteria",
        "or Up": "Terrace",
        "or Down": "Waiting_Area"
    },
    "Terrace": {
        "Jump": "Death",
        "or Back": "Staircase"
    },
    "Waiting_Area": {
        "Up": "Staircase",
        "or Exit": "Exit",
        "or Right": "Morgue",
        "or Left": "Operating_Room",
        "or Inspect": "Find pepper Spray"
    },
    "Operating_Room": {
        "Back": "Waiting_Area",
        "Accept": "Death",
        "Deny": {
            "Crowbar": "No Death",
            "Run": "Death",
            "Bug_Spray": "Death"
        }
    },
    "Morgue": {
        "Body": "Unlock a letter",
        "or Buzzing": "Death",
        "or Back": "Waiting_Area"
    },
    "Exit": {
        "Back": "Waiting_Area",
        "or Try": "Finish"
    }
}

inventory = []


# functions

def white_room():
    location = "White_Room"
    direction = ""

    inventory.clear()
    print()
    print()

    print()
    possible_moves = rooms[location].keys()
    print("possible moves:", *possible_moves)

    direction = input("What will you do? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "door":
        print()
        corridor()
    elif direction == "inspect":
        print()
        time.sleep(1)
        input("It’s plain, clean, and impersonal.")
        input("You can’t jump out of the window; it’s grilled shut.")
        input("The walls are clean, immaculate. The floor— pristine. The bed is always made. ")
        input("No matter how much you destroy the place, it reverts back to its original state.")
        white_room()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print("Please enter valid statements")
        print()
        print()
        white_room()


def corridor():
    location = "Corridor"
    direction = ""

    print()
    time.sleep(1)
    print("_______________________")
    print("_______________________")
    print("You are in the", location)
    print()
    print()
    time.sleep(1)
    input("It is a long, straight hallway. White floors, white walls.")
    input("To the left is the bathroom. To the right, the cafeteria.")
    print()

    print()
    possible_moves = rooms[location].keys()
    print("possible moves:", *possible_moves)

    direction = input("Move which direction? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "left":
        print()
        print()
        bathroom()
    elif direction == "right":
        print()
        print()
        cafeteria()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        corridor()


def bathroom():
    location = "Bathroom"
    direction = ""

    print()
    time.sleep(1)
    print("You are in the", location)
    print()
    print()
    time.sleep(1)
    input("A row of toilet stalls. A mirror. Sinks. A ghost that knocks.")
    input("...")
    input("*knock*")
    input("*knock* *knock*")
    input("You never did put a ghost in this bathroom, at least not consciously.")
    input("But it’s always there now. In the last stall. Each time you come in.")
    input("...")
    print("\nWhat do you do? Investigate the knocking or Head Back (go back to corridor) \n")
    print()
    time.sleep(1)
    possible_moves = rooms[location].keys()
    print("Possible moves:", *possible_moves)

    direction = input("Decision? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "back":
        print()
        print()
        corridor()
    elif direction == "investigate":
        print()
        print()
        bathroom_ex()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        bathroom()


def bathroom_ex():
    location = "Bathroom Stall"
    direction = ""

    print()
    time.sleep(1)
    print("You are in the", location)
    print()
    time.sleep(1)
    input("A young girl, holding out two cards. One red and One blue.")
    input("Her empty BLACK eyes peak at your soul from the fringes of her BLACK hair. ")
    input("She asks you to choose. But regardless of your choice, you die each time.")
    print()
    input("Maybe you should try something new.")
    print()
    print()
    answer = input("Which color do you choose? \n>> ").lower().strip()

    if answer == "red":
        print()
        time.sleep(1)
        input("You knew it was coming, but still flinched when she stabs you. ")
        print()
        input("Her Black eyes still haunt your memories.")
        print()
        print("Maybe Red isn’t the answer.")
        input("(Press Enter to Continue...)")
        print()
        print()
        input("You wake up in the white room.")
        white_room()

    elif answer == "blue":
        print()
        time.sleep(1)
        input("You knew it was coming, but still flinched when she strangles you.")
        input()
        print("Her Black eyes still haunt your memories.")
        print()
        print("Maybe Blue isn’t the answer.")
        input("(Press Enter to Continue...)")
        print()
        print()
        input("You wake up in the white room.")
        white_room()

    elif answer == "black":
        print()
        time.sleep(1)
        input("Ah. Interesting. You choose a completely different color.")
        input("Slowly, she turns her head to the side, not stopping until it did a complete 180 degree turn.")
        input("You let your eyes focus on the back of her head, and notice the letter 'R' written on it")
        print()
        print("You get a feeling that this is important.")
        print()
        input("Seeing as nothing more happened, you head back to the corridor.")
        print()
        print()
        corridor()

    elif answer == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        bathroom_ex()


def cafeteria():
    location = "Cafeteria"
    direction = ""

    print()
    time.sleep(1)
    print("You are in the", location)
    print()
    time.sleep(1)
    input("It seems to be connected to the stairway.")
    input("As you enter, you see the menu.")
    print("    —— —— —— —— —— —— —— ")
    print("    |       menu       |")
    print("    | 1)juIce          |")
    print("    | 2)pIzza          |")
    print("    | 3)Ice cream      |")
    print("    | 4)rIce           |")
    print("    | 5)chIcken wIngs  |")
    print("    —— —— —— —— —— —— —— ")
    time.sleep(0.7)
    input("How peculiar... The letter ‘I’ stands out.")
    print()
    input("Behind the counter you see a wide variety of...")
    input("Human organs...")
    input("You don’t know why. But looking at it makes your stomach hurl each time. ")
    print()

    answer1 = input("What do you do? \n>Run to the staircase! \n>Eat the organs! \n>Go Back to Corridor! \n(Type Run or Eat or Back) \n>> ").lower().strip()

    if answer1 == "run":
        print()
        time.sleep(1)
        input("The sight of the 'food' still makes you uncomfortable.")
        print("Perhaps you could go up for some fresh air or go down.")
        print()
        print()
        staircase()
    elif answer1 == "eat":
        print()
        time.sleep(1)
        input("You don’t understand what compels you to do this.")
        input("But you eat the organs.")
        print()
        input("You wake up in the white room. The feeling of nausea won’t leave you.")
        print()
        input("Maybe cannibalism isn't the answer.")
        input("...")
        white_room()
    elif answer1 == "back":
        print()
        time.sleep(1)
        corridor()
    elif answer1 == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        cafeteria()


def staircase():
    location = "Staircase"
    direction = ""

    print()
    time.sleep(0.7)
    print("You are in the", location)
    print()
    time.sleep(0.7)
    print()
    possible_moves = rooms[location].keys()
    print("Possible moves:", *possible_moves)

    direction = input("Move which direction? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "up":
        time.sleep(1)
        take_crowbar()
    elif direction == "down":
        print()
        print()
        waiting_area()
    elif direction == "back":
        print()
        print()
        cafeteria()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        staircase()


def take_crowbar():
    while 'crowbar' not in inventory:
        print()
        print()
        print()
        input("On the way up the stairs, something catches your eye.")
        input("It's a Crowbar! ")
        input("Should you take it? ")
        input("But what could you possibly use it for?")
        print()
        print()
        print("Pick it up?")
        take_the_crowbar = input("Yes/No: \n>> ").lower().strip()

        if take_the_crowbar == "yes":
            add_to_inventory("crowbar")
            time.sleep(0.5)
            print("CROWBAR added to inventory")
            time.sleep(0.5)
            print("Inventory:")
            print(inventory)
            print()
            terrace()
        elif take_the_crowbar == "no":
            print("You leave the Crowbar in the Terrace.")
            input("...")
            print()
            terrace()
        elif take_the_crowbar == "quit":
            print("")
            time.sleep(1)
            quit("GAME TERMINATING...")
        else:
            print()
            print("Invalid move! \nOnly Enter Valid Statements.")
            take_crowbar()
    terrace()


def terrace():
    location = "Terrace"
    direction = ""

    print()
    print()
    time.sleep(1)
    print("* ,   . +   `. *` . . +,   *  ` . + ,  . `  .")
    print("  .  *  ` . + ,  . `  .   . +   `. *` . . + `")
    print("You are in the", location)
    time.sleep(1)
    input("The stars look pretty tonight.")
    input("You wonder what exactly you're doing here.")
    input("You're not sure what exactly you want to do either.")
    input("Would you like to go back downstairs or...")
    print()

    print()
    possible_moves = rooms[location].keys()
    print("Possible moves:", *possible_moves)

    direction = input("Decision? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "back":
        print()
        time.sleep(1)
        input("As tempting as a trip to the stars sounds like, you decide to keep fighting.")
        input("You could come back here anytime, anyway.")
        print()
        print()
        staircase()
    elif direction == "jump":
        print()
        time.sleep(1)
        print("Do you really wish to jump? Nothing special would happen. You’ll just die.")
        input("As always wake up in the white room.")
        input("Maybe it's different this time...")
        input("You brace yourself and fall forward.")
        print()
        time.sleep(1)
        input("... Only to wake up in the White Room.")
        print()
        print("God dammit.")
        input("Same thing, again and again.")
        print()
        print()
        white_room()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        terrace()


def waiting_area():
    location = "Waiting_Area"
    direction = ""

    while direction != "exit":

        print()
        time.sleep(0.7)
        print("You are in the", location)
        print()
        time.sleep(0.7)
        input("The deeper levels always felt strange to you.")
        input("The Waiting Area is nothing much, except for the safe locker.")
        input("To the left is an operating room and to the right... a morgue.")
        input("There’s also a supply closet.")
        print("You may also go back up the staircase. (Type 'up')")
        print()

        time.sleep(0.7)
        print()
        possible_moves = rooms[location].keys()
        print("possible moves:", *possible_moves)

        direction = input("Move which direction? \n>> ").lower().strip()
        print("You entered:", direction)

        if direction == "left":
            print()
            print()
            operation_room()
        elif direction == "up":
            print()
            print()
            staircase()
        elif direction == "right":
            print()
            print()
            morgue()
        elif direction == "exit":
            print()
            print()
            password()
        elif direction == "inspect":
            if 'bug spray' not in inventory:
                print()
                time.sleep(1)
                input("You navigate your way through the chairs.")
                input("You see a door that leads to the cleaning closet.")
                input("In there you find a bottle of bug spray.")
                print()
                take_spray()
            elif 'bug spray' in inventory:
                print()
                time.sleep(1)
                print("There is nothing left to inspect.")
                print()
                print()
                waiting_area()
            elif direction == "quit":
                print("")
                time.sleep(1)
                quit("GAME TERMINATING...")
        elif direction == "quit":
            print("")
            time.sleep(1)
            quit("GAME TERMINATING...")
        else:
            print()
            print("Invalid move! \nOnly Enter Valid Statements.")
            print()
            print()
            waiting_area()


def take_spray():

    print("Pick it up?")
    take_the_spray = input("Yes/No: \n>> ").lower().strip()
    if take_the_spray == "yes":
        add_to_inventory("bug spray")
        print()
        time.sleep(0.5)
        print("Bug spray added to inventory")
        print()
        time.sleep(0.5)
        print("Inventory:")
        print(inventory)
        print()
        input("You head back to the waiting_area")
        print()
        print()
        waiting_area()
    elif take_the_spray == "no":
        print()
        input("You leave the Bug spray in the cabinet.")
        input("You head back to the waiting_area")
        print()
        print()
        waiting_area()
    elif take_the_spray == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        take_spray()



def operation_room():
    location = "Operating_Room"
    direction = ""

    time.sleep(1)
    print("You are in the", location)
    print()
    time.sleep(1)
    input("'The Mad Surgeon', as you’ve come to call him, greets you.")
    input("He wears his scrubs and a face mask and a face shield.")
    input("He asks you if you want to get rid of your depression.")
    input("What a concept. But maybe it’s worth another shot...")
    input("All you know is that you can't kill him, but you can stall for time.")
    input("Every time he 'dies', it only takes him a few minutes to come back to life.")
    input("Looks like he's alive again.")
    print()
    input("You can go Back to the Waiting_Area")
    print()

    print("Possible moves: ", "Accept,", "Deny", " or Back")

    direction = input("What do you do? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "back":
        print()
        print()
        waiting_area()
    elif direction == "accept":
        print()
        input("You lay on the bench, telling yourself that maybe this time he can actually cure you.")
        input("...")
        input("You sigh as you hear him laugh. The Mad Surgeon tells you that all he wants from you are your organs.")
        input("He congratulates you for being stupid enough to think anything could cure you.")
        input("You hope you won’t wake up in the White Room again.")
        print()
        input("But of course, you do.")
        white_room()
    elif direction == "deny":
        deny()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        operation_room()


def deny():

    print()
    time.sleep(1)
    input("The surgeon charges at you with a scalpel.")
    print()
    print("Possible moves: 'Inventory' or 'Run'")
    decide = input("Quick! What do you do?: \n>>").lower().strip()

    if decide == "inventory":
        print()
        print(inventory)
        if not inventory:
            print()
            time.sleep(1)
            input("Uh-oh. Looks like you have nothing to defend yourself with.")
            print("Only thing you can do now, is run.")
            print("So you turn around and try to run")
            print("But he catches up with you.")
            print()
            time.sleep(1)
            print("You wake up in the white room.")
            input("Maybe next time you should find something to defend yourself with...")
            print()
            print()
            white_room()
        else:
            defend = input("Pick something to defend yourself with. \n>> ").lower().replace(" ","")
            if defend == "crowbar":
                print()
                time.sleep(1)
                input("The surgeon tries to stab you with his scalpel.")
                input("You block his attacks.")
                input("You delt him a deadly blow with your crowbar and watch as his body flops to the ground.")
                print()
                input("You notice his ID card.")
                input("It has the letter 'B' written on it.")
                print()
                input("Feeling a little shaky, you return to the Waiting_Area")
                print()
                print()
                waiting_area()
            elif defend == "bugspray":
                time.sleep(1)
                input("The surgeon tries to stab you with his scalpel.")
                input("You use the bug spray, but realize how ineffective it is against his surgical mask and face shield")
                input("How stupid! You try to run away, but he catches up to you.")
                input("You were unable to make it out alive.")
                print()
                input("You wake up in the white room, yet again.")
                print()
                white_room()
            elif defend == "quit":
                print("")
                time.sleep(1)
                quit("GAME TERMINATING...")
            else:
                print()
                print("Invalid move! \nOnly Enter Valid Statements.")
                print()
                print()
                deny()
    elif decide == "run":
        time.sleep(1)
        print()
        input("The surgeon tries to stab you with his scalpel.")
        input("You turn around and try to run,")
        input("But you couldn't make it in time.")
        print()
        input("You wake up in the white room.")
        print()
        white_room()
    elif decide == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        deny()


def morgue():
    location = "Morgue"
    direction = ""

    print("You are in the", location)

    print()
    time.sleep(1)
    input("The Lights Flicker.")
    input("This place gives you a bad vibe")
    input("There’s a body on the stretcher. A white sheet covers it.")
    input("The blood seeps through the fabric.")
    input("The foot is uncovered. You can see the toe tag.")
    input("At the same time, you hear a sharp buzzing sound.")
    print()
    input("*Buzzzzzz*")
    print()
    input("It originates from one of the body storage cabinets.")
    print()
    print("What do you do? Inspect the Body or the Buzzing?")
    print("(You may also go back to the Waiting_Area)")

    time.sleep(0.6)
    print()
    print()
    possible_moves = rooms[location].keys()
    print("Possible moves:", *possible_moves)

    direction = input("Decision? \n>> ").lower().strip()
    print("You entered: ", direction)

    if direction == "back":
        print()
        print()
        waiting_area()
    elif direction == "body":
        print()
        time.sleep(1)
        input("You cautiously make your way towards the body.")
        input("Upon closer inspection, you notice that the foot is decomposing.")
        input("The toe tag seems to be covered in mud. How unusual.")
        input("You reach forward to dust off the mud.")
        print()
        input("Suddenly, the body sits up.")
        print()
        print("Scared to death, you run back to the waiting room.")
    elif direction == "buzzing":
        print()
        buzz()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        morgue()


def buzz():
    print()
    time.sleep(1)
    input("You head towards the cabinet wondering what's causing that noise.")
    input("It stops; you don't hear a thing.")
    input("Something's fishy and you know it, but you open the cabinet anyway.")
    print()
    input("*Buzzzzzz*")
    print()
    input("Before you realize, a swarm of bluebottle flies surround you.")
    input("\"It's just flies,\" you think.")
    input("Something feels off. But what?")
    print("It's your skin.")
    time.sleep(0.6)
    input("Crap. They are feeding on your skin!")
    print()
    print()

    print("Possible moves: Inventory or run")
    decide = input("What do you do? \n>> ").lower().strip()

    if decide == "inventory":
        print()
        print(inventory)
        if not inventory:
            print()
            time.sleep(1)
            input("Uh-oh. Looks like you have nothing to defend yourself with.")
            input("Only one thing left to do.")
            input("You turn around and run,")
            input("But you can't get through. It's an impenetrable swarm of flies.")
            input("You try but you get eaten to death by those flies.")
            print()
            print()
            print("You wake up in the white room.")
            input("Maybe next time you should find something to defend yourself with...")
            print()
            print()
            white_room()
        elif decide == "quit":
            print("")
            time.sleep(1)
            quit("GAME TERMINATING...")
        else:
            defend = input("Pick something to defend yourself with. \n>> ").lower().replace(" ","")
            if defend == "bugspray":
                print()
                time.sleep(1)
                input("The flies won't leave you alone.")
                input("So you use the bugspray to kill 'em.")
                input("You spray it all over the room and watch as they rain down to the ground.")
                input("A simple, but effective solution.")
                print()
                input("Once the last of them die, you notice a piece of paper in the cabinet.")
                input("It has the letter 'D' written on it.")
                print()
                input("You get the feeling that this is important. You return to the Waiting Area.")
                input("...")
                print()
                print()
                waiting_area()
            elif defend == "crowbar":
                print()
                time.sleep(1)
                input("The swarm of flies dive on to you.")
                input("You use the crowbar, but realize that the flies just escapes your every hit.")
                input("How stupid! You try to run away, but it's of no use")
                input("You get eaten up to death by those flies.")
                print()
                input("You wake up; again in the white room.")
                print()
                white_room()
            elif defend == "quit":
                print("")
                time.sleep(1)
                quit("GAME TERMINATING...")
            else:
                print()
                print("Invalid move! \nOnly Enter Valid Statements.")
                print()
                print()
                buzz()
    elif decide == "run":
        print()
        time.sleep(1)
        input("The swarm of flies dive on to you.")
        input("You turn around and try to run")
        input("But you just can't get through it.")
        input("And you get eaten up to death by those flies.")
        print()
        print()
        input("You wake up in the white room.")
        print()
        print()
        white_room()
    elif decide == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        buzz()


def password():
    location = "Exit"
    direction = ""

    print()
    time.sleep(1)
    print("You are at the", location, ". Or you hope it is.")
    print()
    time.sleep(1)
    input("There's a safe with a FOUR letter code.")
    print("Do you wish to try? Remember, you have a limited amount of attempts.")
    input("Head Back if you think you aren't ready.")
    print()

    print()
    possible_moves = rooms[location].keys()
    print("possible moves:", *possible_moves)

    direction = input("Your choice? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "back":
        print()
        print()
        waiting_area()
    elif direction == "try":
        word = "bird"
        time.sleep(1)
        print("REMEMBER, you have 2 attemps only.")
        time.sleep(1)
        guess = input("\nGuess the 4-letter word: ").lower().strip()
        tries = 1
        if guess != word:
            print("\nINCORRECT PASSWORD.")
            print("Try again, and get it right if you wish to live.")
            tries += 1
            guess = input("\nGuess the 4-letter word: ")
        if guess != word and tries == 2:
            print()
            print("\nINCORRECT PASSWORD")
            time.sleep(0.3)
            input("You got it wrong!")
            print()
            input("\nA tiny part of you wished that this meant you would die. For real.")
            input("But reality is often disappointing.")
            print()
            input("You're back at the White Room again.")
            print()
            input("Just like every other time.")
            input("Death just doesn't seem to exist here.")
            print()
            print()
            white_room()
        print()
        print("CORRECT PASSWORD")
        print()
        safe()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        password()


def safe():
    print()
    time.sleep(1)
    input("You open the safe, smiling, hoping for something good to happen.")
    input("Inside, you see a locket; it was your mom's. It has a picture of us together.")
    time.sleep(0.3)
    input("It was the only thing that was left of hers.")
    print()
    print("//FLASHBACK//")
    time.sleep(0.6)
    input("She used to suffer from nightmares, something similar to yours.")
    input("But she was brave enough to resist. She even managed to overcome it.")
    input("Perhaps you’re just not strong enough...")
    input("You remember... She used to say:")
    time.sleep(0.6)
    print("     \"My little bird, I hope when you take that leap")
    print("       of faith, you have nothing to fear anymore...\"")
    time.sleep(1)
    input("//FLASHBACK END//")
    print()
    time.sleep(1)
    input("A leap of faith...")
    time.sleep(0.7)
    input("A leap... a Jump...?!")
    input("Is that what it means?")
    input("Maybe...")
    print()
    print("But I’ve tried jumping off the terrace. Maybe more than a hundred times.")
    input("It always ends in the White Room.")
    print()
    input("Well. There can’t be any harm in trying once more.")
    input("It might be different.")
    print()
    input("You head straight to the terrace.")
    print()
    print()
    terrace_alt()


def terrace_alt():
    location = "Terrace"
    direction = ""

    print()
    time.sleep(1)
    print("* ,   . +   `. *` . . +,   *  ` . + ,  . `  .")
    print("  .  *  ` . + ,  . `  .   . +   `. *` . . + `")
    print("You are in the", location)
    time.sleep(1)
    input("This is it.")
    input("You take one last look at the stars.")
    input("You could jump... Or you could head back.")
    input("But you've exhausted every inch of this nightmare.")
    input("There is no point in heading back.")
    print()
    print("Possible moves: Stay or Jump")

    direction = input("Decision? \n>> ").lower().strip()
    print("You entered:", direction)

    if direction == "stay":
        print()
        time.sleep(0.6)
        input("Alright. No.")
        input("You don't want to jump. Not right now, at least.")
        input("You could come back here anytime, anyway.")
        print()
        input("Right...?")
        print()
        input("... It doesn't feel right though...")
        print()
        print("Nevertheless, you leave.")
        print("On the way downstairs, you feel your vision black out.")
        print()
        input("You slowly come to yourself.")
        input("You're in a white room. The White Room.")
        print()
        print("You squeeze your eyes shut. It shouldn't be happening. No, not after everything— just to come back here—")
        print("But what else did you expect? You did nothing different.")
        input("You were a coward who didn't take the chance to change.")
        print()
        input("You’re stuck. You can’t get out.")
        input("It’s a dream. It’s a nightmare.")
        time.sleep(0.4)
        print("It’s a nightmare. You’re stuck.")
        time.sleep(0.4)
        print("You’re stuck.")
        time.sleep(0.3)
        print("You’re stuck. You’re stuck. You’re stuck.")
        time.sleep(0.2)
        print("You’re stuck. You’re stuck. You’re stuck. You’re stuck. You’re stuck. You’re stuck.")
        time.sleep(0.1)
        print("Stuck. Stuck. Stuck. Stu—")
        input("...")
        print()
        print()
        print()
        print()
        print("------------------------")
        print("| ENDING 2/2: INSANITY |")
        print("------------------------")
        print()
        print()
        print()
        print()
        time.sleep(1)
        print("You couldn't make it out.")
        input("You stayed, despite knowing there was a way out.")
        input("Your grief and thoughts weigh you down.")
        input("You wonder if you could have done anything differently.")
        print()
        input("If you had been brave.")
        print()
        input("Maybe things would have been better...")
        print()
        print()
        restart_seq()

    elif direction == "jump":
        print()
        input("You brace yourself, and fall forward.")
        print()
        print()
        input("You slowly come to yourself, waking up in a white room.")
        input("A white room? /The/ white room?")
        print("You squeeze your eyes shut. It couldn’t be happening. No, not after everything— just to come back here—")
        time.sleep(0.5)
        print("*knock*")
        time.sleep(0.2)
        input("*knock*")
        input("Someone walks in through the door— a man— a man that you recognize.")
        input("A man from the hospital— the one you were in before the dream.")
        print()
        input("This isn't a part of the dream. It’s not the dream— is it the dream?")
        input("It can’t be. There are in people here. Real people you haven’t seen in your dreams. ")
        print()
        print()
        print("The nurse asks you if you've been sleeping well.")
        print("You nod.")
        print()
        print()
        input("You search for your mother's locket on your bedside table.")
        input("It's there. You see two faces smiling at one another.")
        print()
        input("You carefully rip the picture until only your mother’s face remains, and place it back into the locket.")
        input("Your mother lives in dreams. You belong here.")
        print()
        input("You’re not sure when you’re going to be okay... but that’s okay.")
        input("It might take a while, but you will make it out of this hospital.")
        input("With a full recovery.")
        input("You won’t get stuck.")
        input("You look at your mother one last time before you close the locket with a click.")
        print()
        print()
        print()
        print()
        print("-----------------------")
        print("| ENDING 1/2: CLOSURE |")
        print("-----------------------")
        print()
        print()
        print()
        time.sleep(1)
        input("It was the fear of being stuck in a hospital that put you in an endless loop of actually being stuck.")
        input("After coming to terms with yourself, you realize that it might take a while for you to be alright.")
        input("But you know it’ll happen someday.")
        print()
        print()
        print("Congratulations! You made it!")
        print()
        print()
        restart_seq()
    elif direction == "quit":
        print("")
        time.sleep(1)
        quit("GAME TERMINATING...")
    else:
        print()
        print("Invalid move! \nOnly Enter Valid Statements.")
        print()
        print()
        terrace_alt()


def add_to_inventory(item):
    inventory.append(item)


def restart_seq():
    print()
    answer1 = input("Replay Game? (Yes/No) \n>> ").lower().strip()
    if answer1 == "yes":
        print(""*5)
        print("RESTARTING...")
        print()
        print()
        print("You're back here again.")
        print("You know it's a dream, that’s for sure.")
        print()
        time.sleep(1)
        input("(Press Enter to Continue...)")
        input("But you're stuck here. Stuck for too long.")
        input("You can't control all of it. It feels like it's the dream that controls you.")
        input()
        print("You are trapped in this twisted hospital")
        print("You can't wake up. You can't die. If you die, you wake up back in this room.")
        input()
        input("All you want is to be freed.")
        print()
        print()
        time.sleep(0.7)
        print("A white room. A single bed. One window. ")
        input("There is a door that leads to the corridor.")
        white_room()

    elif answer1 == "no":
        print("Thank you for playing :)")
        quit()
    else:
        print()
        print("Sorry, I don't understand. English please!")

        print()
        print()
        restart_seq()


# call stuff

print()
print()
print()
print("********************")
print("*   LUCID DREAMS   *")
print("********************")
print()
print()
print()
time.sleep(1)
print("Welcome!")
time.sleep(1)
print("The rules of the game are simple. Type the command from given options. Find a way to escape.")
time.sleep(2)
print("GAME LOADING...")
time.sleep(1)
print("TIP: use lower-case characters only")
time.sleep(2)
print("LOADING...")
time.sleep(0.7)
print("You always have 'quit' option to exit game")
time.sleep(2)
print("STARTING GAME...")
print()
print()
print()
time.sleep(1)
input("(Press Enter to Continue...)")
print()
input("You're back here again.")
input("You know it's a dream, that’s for sure.")
input("But you're stuck here. Stuck for too long.")
input("You can't control all of it. It feels like it's the dream that controls you.")
input("You are trapped in this twisted hospital.")
input("You can't wake up. You can't die. If you die, you wake up back in this room.")
print()
input("All you want is to be freed.")
print()
print()
time.sleep(0.7)
print("A white room. A single bed. One window. ")
input("There is a door that leads to the corridor.")

white_room()
