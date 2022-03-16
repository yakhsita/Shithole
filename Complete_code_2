# a text-based adventure game set in a hospital

from tkinter import *
from tkinter.ttk import *
from tkinter import font
import tkinter as tk

inventory = []


root = Tk()
root.geometry("800x700")
root['bg'] = 'black'
root.resizable(0,0)

canvas = Canvas(root, height=700, width=800)
canvas.pack()


# ------------------------------------------------- Storage --------------------------------------------------------- #

#1 logo frame <- first pg
frame = tk.Frame(root, bg="black")
frame.place(relwidth=1, relheight=1)

photo = PhotoImage(file = "H:\Backgroundd.png")
photo_label = tk.Label(frame, image=photo, bg='black') # making the image into a label
photo_label.place(x=-2, y=-2)


# frame1 stuff
f1_img = PhotoImage(file = "H:\Welcomee.png")
f1_pic_label = tk.Label(frame, image=f1_img, bg="black")
w = tk.Label(root, text='WELCOME!', bg='black', fg='white', font=('Times', 50))
r = tk.Label(root,
             text=' The rules of the game are simple.\nChoose the command from given options.\nFind a way to escape.',
             bg='black', fg='white', font=('Times New Roman', 15), justify='center')


# frame2 <-- loading
#f2_img = PhotoImage(file = "H:\Loadingg.png")
#f2_pic_label = tk.Label(frame, image=f2_img, bg="black")
g = tk.Label(frame, text="Game loading . . .", bg='black', fg='white', font=('Times New Roman', 30, 'bold'), border=3)
dots = " ... "

# frame3 stuff <-- Intro
f3_img = PhotoImage(file = "H:\Introo.png")
f3_pic_label = Label(frame, image=f3_img)
y = tk.Label(frame, text="You're back here again. \nYou know it's a dream, that’s for sure.\nBut you're stuck here. Stuck for too long.\nYou can't control all of it.\n It feels like it's the dream that controls you. \nYou are trapped in this twisted hospital.\n You can't wake up. You can't die.\n If you die, you wake up back in this room.\n\nAll you want is to be freed.",
                 font=("Times New Roman", 15), justify="center", bg="black", fg="white")


# frame4 stuff <-- whiteroom
f4_img = PhotoImage(file = "H:\Whiteroomm.png")
b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2, command=root.destroy)
f4_pic_label = tk.Label(frame, image=f4_img)
y1 = tk.Label(frame, text="A white room.\nA single bed. One window.\nThere is a door that leads to the corridor.",
                 font=("Bell MT", 18), justify="center", bg="black", fg="white")


# frame5 stuff <-- Inspect
f5_img = PhotoImage(file = "H:\Inspectt.png")
f5_pic_label = Label(frame, image=f5_img)
y2 = tk.Label(frame, text="It’s plain, clean, and impersonal.\nYou can’t jump out of the window; it’s grilled shut.\nThe walls are clean, immaculate. The floor— pristine.\nThe bed is always made. No matter how much you destroy the place,\nit reverts back to its original state.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white", borderwidth=0)


# frame6 stuff <-- corridor
f6_img = PhotoImage(file = "H:\Corridorr.png")
f6_pic_label = Label(frame, image=f6_img)
y3 = tk.Label(frame, text="The door opens to a corridor. \nTo the left is the bathroom.\nTo the right, the cafeteria.\n\nMove which direction?",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white", border=0)


# frame7 stuff <-- Left(Bathroom)
f7_img = PhotoImage(file = "H:\Bathroomm.png")
f7_pic_label = tk.Label(frame, image=f7_img)
y4 = tk.Label(frame, text="A row of toilet stalls. A mirror. Sinks. A ghost that knocks. \n*knock* *knock* *knock* \nThe ghost is always there. In the last stall. Each time you come in. \n\nNext Move?",
                 font=("Times New Roman", 17), justify="center", bg="black", fg="white")


# frame8 stuff <-- Inspect Knocking
f8_img = PhotoImage(file = "H:\Toilett.png")
f8_pic_label = tk.Label(frame, image=f8_img)
y5 = tk.Label(frame, text="You Reach the last stall. A girl holds out two cards; one red, one blue. \nHer empty BLACK eyes peak at your soul from the fringes of her BLACK hair.\nShe asks you to choose. But regardless of your choice, you die each time.\nMaybe you should try something new...",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame9a stuff <-- Red Colour
f9a_img = PhotoImage(file = "H:\Redtoilett.png")
f9a_pic_label = tk.Label(frame, image=f9a_img)
y6 = tk.Label(frame, text="You knew it was coming, but you still flinched when she stabs you.\nHer Black eyes still haunt your memories.\nMaybe Red isn’t the answer. \n\nYou wake up in the White Room.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame9b stuff <-- Blue Colour
f9b_img = PhotoImage(file = "H:\Bluetoilett.png")
f9b_pic_label = tk.Label(frame, image=f9b_img)
y7a = tk.Label(frame, text="You knew it was coming, but you still struggled when she strangles you.\nHer Black eyes still haunt your memories.\nMaybe Blue isn’t the answer.\n\nYou wake up in the White Room.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame9c stuff <-- Black Colour
f9c_img = PhotoImage(file = "H:\Blacktoilett.png")
f9c_pic_label = tk.Label(frame, image=f9c_img)
y7b = tk.Label(frame, text="Ah. Interesting. You choose a completely different color.\nSlowly, she turns her head to the side, not stopping until it did a complete 180 degree turn.\nYou let your eyes focus on the back of her head, and notice the letter 'R' written on it.\nYou get a feeling that this is important.\nSeeing as nothing more happened, you head back to the corridor.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame10 stuff <-- Right(Cafeteria)
f10_img = PhotoImage(file = "H:\Menuu.png")
f10_pic_label = tk.Label(frame, image=f10_img)
y7c = tk.Label(frame, text="You find yourself in the Cafeteria.\nIt is connected to the Stairway\nAt the entrance, you see the menu.\nThe letter 'I' sticks out, how weird.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame11 stuff <-- inspect(In Cafeteria)
f11_img = PhotoImage(file = "H:\Meatt.png")
f11_pic_label = tk.Label(frame, image=f11_img)
y8 = tk.Label(frame, text="Behind the counter, you see that the 'food' here is just human organs.\nThe sight of it makes you hurl each time.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame12 stuff <-- Eat organs
f12_img = PhotoImage(file = "H:\Deathh.png")
f12_pic_label = tk.Label(frame, image=f12_img)
y9 = tk.Label(frame, text="You don’t understand what compels you to do this.\nBut you eat the organs.\nNext thing you know, you wake up in the white room. \nThe feeling of nausea won’t leave you.\nMaybe cannibalism isn't the answer.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame13 stuff <-- Run to the stairs(From the cafeteria)
f13_img = PhotoImage(file = "H:\Stairss.png")
f13_pic_label = tk.Label(frame, image=f13_img)
y10 = tk.Label(frame, text="You are in the staircase.\nGo where?",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white", borderwidth=0, border=0)


# frame14 stuff <-- Up(Crowbar)
f14_img = PhotoImage(file = "H:\Crowbarr.png")
f14_pic_label = Label(frame, image=f14_img)
y11 = tk.Label(frame, text="You found a Crowbar on the way up.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white", wraplength=300)


# frame15 stuff <-- Terrace
f15_img = PhotoImage(file = "H:\Terracee.png")
f15_pic_label = Label(frame, image=f15_img)
y12 = tk.Label(frame, text="You are in the Terrace.\nThe Stars look very pretty.\nYou're not sure what exactly you're doing.\nWould you like to go back downstairs or...",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white", wraplength=400)


# frame16 stuff <-- Jump(From Terrace)
f16_img = PhotoImage(file = "H:\Jumpp.png")
f16_pic_label = Label(frame, image=f16_img)
y13 = tk.Label(frame, text="You glanced over the edge, and jumped off.\nYou knew nothing special would happen.\nYou died and woke up in the white room.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame17 stuff <-- Inspect(In Waiting_area)
f17_img = PhotoImage(file = "H:\Cabinett.png")
f17_pic_label = Label(frame, image=f17_img)
y14 = tk.Label(frame, text="You navigate your way through the chairs. You see a door that leads to the cleaning closet. In there you find a bottle of bug spray.\n",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white", wraplength=300)


# frame18 stuff <-- Waiting_area(Down from staircase)
f18_img = PhotoImage(file = "H:\Waitingareaa.png")
f18_pic_label = Label(frame, image=f18_img)
y15 = tk.Label(frame, text="You are in the Waiting Area.\nThe deeper levels always felt strange to you.\nTo the left is an operating room and to the right... a morgue.\nIn front of you is the 'exit',\nwhere the safe locker is located.\nThere’s also a supply closet.\nMove which direction?",
                 font=("Times New Roman", 17), justify="center", bg="black", fg="white")


# frame19 stuff <-- Operation_Theater(Left)
f19_img = PhotoImage(file = "H:\Surgeonn.png")
f19_pic_label = Label(frame, image=f19_img)
y16 = tk.Label(frame, text="You are in the Operation Theater.\n'The Mad Surgeon', as you’ve come to call him, greets you. He asks you if you want to get rid of your depression. What a concept. But maybe it’s worth another shot... All you know is that every time he 'dies', it only takes him a few minutes to come back to life. Looks like he's alive again.\nWhat do you do?",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white", wraplength=400)


# frame20 stuff <-- Accept
f20_img = PhotoImage(file = "H:\Acceptt.png")
f20_pic_label = Label(frame, image=f20_img)
y17 = tk.Label(frame, text="You lay on the bench and sigh as you hear him laugh. The Mad Surgeon tells you\nthat all he wants from you are your organs.\nHe congratulates you for being stupid\nenough to think anything could cure you.\nYou hope you won’t wake up in the White Room again.\n\nBut of course, you do.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# frame21 stuff <-- Inventory(with crowbar)
f21_img = PhotoImage(file = "H:\Idcardd.png")
f21_pic_label = Label(frame, image=f21_img)
y18 = tk.Label(frame, text="Furious, the surgeon tries to stab you with his scalpel.\nYou block his attacks.\nYou delt him a deadly blow with your crowbar and\nwatch as his body flops to the ground. You notice his ID card.\nIt has the letter 'B' written on it.\nFeeling a little shaky, you return to the Waiting_Area.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame22 stuff <-- Inventory(without crowbar)
f22_img = PhotoImage(file = "H:\Withoutcroww.png")
f22_pic_label = Label(frame, image=f22_img)
y19 = tk.Label(frame, text="Furious, the surgeon charges at you with a scalpel.\nUh-oh. Looks like you have nothing to defend yourself with.\nOnly thing you can do now, is run.\nSo you turn around and try to run,\nBut he catches up with you.\nMaybe next time you should find something to defend yourself with...",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# frame23 stuff <-- Morgue(right)
f23_img = PhotoImage(file = "H:\Morguee.png")
f23_pic_label = Label(frame, image=f23_img)
y20 = tk.Label(frame, text="The Lights Flicker.\nThis place gives you a bad vibe.\nThere’s a body on the stretcher. A white sheet covers it.\nThe blood seeps through the fabric.\nThe foot is uncovered. You can see the toe tag.\nAt the same time, you hear a sharp buzzing sound.\n*Buzzzzzz*\nIt originates from one of the body storage cabinets.\nWhat do you do? Inspect the Body or the Buzzing?",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame24 stuff <-- Body(In morgue)
f24_img = PhotoImage(file = "H:\Deadbodyy.png")
f24_pic_label = Label(frame, image=f24_img)
y21 = tk.Label(frame, text="You cautiously make your way towards the body.\nUpon closer inspection, you notice that the foot is decomposing.\nThe toe tag seems to be covered in mud. How unusual.\nYou reach forward to dust off the mud.\nSuddenly, the body sits up.\nScared to death, you run back to the waiting room.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# frame25ha stuff <-- Buzz
f25ha_img = PhotoImage(file = "H:\Fliess.png")
f25ha_pic_label = Label(frame, image=f25ha_img)
y22 = tk.Label(frame, text="You head towards the cabinet wondering what's causing that noise.\nIt stops; you don't hear a thing.\nSomething's fishy and you know it, but you open the cabinet anyway.\n*Buzzzzzz* \nBefore you realize, a swarm of bluebottle flies surround you.\n\"It's just flies,\" you think.\nSomething feels off. But what?\nIt's your skin.\nCrap. They are feeding on your skin!\nWhat do you do?",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white", wraplength=400)

# frame25 stuff <-- Buzzing(Inventory)(without bugspray)
f25_img = PhotoImage(file = "H:\Deathh.png")
f25_pic_label = Label(frame, image=f25_img)
y23 = tk.Label(frame, text="Uh-oh. Looks like you never found a bugspray.\nOnly one thing left to do.\nYou turn around and run,\nBut you can't get through. It's an impenetrable swarm of flies.\nYou try but you get eaten to death by those flies.\nYou wake up in the white room.\nMaybe next time you should find something to defend yourself with...",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame26 stuff <-- Buzzing(Inventory)(with bugspray)
f26_img = PhotoImage(file = "H:\Letterdd.png")
f26_pic_label = Label(frame, image=f26_img)
y24 = tk.Label(frame, text="\nThe flies won't leave you alone.\nSo you use the bugspray to kill 'em.\nYou spray it all over the room and watch as they rain down to the ground.\nA simple, but effective solution.\nOnce the last of them die, you notice a piece of paper in the cabinet.\nIt has the letter 'D' written on it.\nYou get the feeling that this is important. You return to the Waiting Area.\n...",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# frame26ha stuff <-- Run
f26ha_img = PhotoImage(file = "H:\Deathh.png")
f26ha_pic_label = Label(frame, image=f26ha_img)
y25 = tk.Label(frame, text="You turn around and run,\nBut you can't get through. It's an impenetrable swarm of flies.\nYou try but you get eaten to death by those flies.\nYou wake up in the white room.\nMaybe next time you should find something to defend yourself with...",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# frame27 stuff <-- Exit
f27_img = PhotoImage(file = "H:\Lockerr.png")
f27_pic_label = Label(frame, image=f27_img)
y26 = tk.Label(frame, text="You are at the Exit. Or you hope it is.\nThere's a safe with a FOUR letter code. Do you wish to try?\nRemember, you have a limited amount of attempts.\nHead Back if you think you aren't ready.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame28 stuff <-- Try
f28_img = PhotoImage(file ="H:\Lockerr.png")
f28_pic_label = Label(frame, image=f28_img)
y27 = tk.Label(frame, text="REMEMBER, you have 1 attemps only.\n\nGuess the 4-letter word",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame29 stuff <-- Try(Entry correct)(In Exit)
f29_img = PhotoImage(file = "H:\Openlockerr.png")
f29_pic_label = Label(frame, image=f29_img)
y28 = tk.Label(frame, text="CORRECT PASSWORD!\n\nInside the safe, you see your mom's locket.\nIt has a picture of us together.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")



# frame30 stuff <-- Try(Entry wrong)(In Exit)
# f30_img = PhotoImage(file = "H:\")
# f30_pic_label = Label(frame, image=f30_img)
y29 = tk.Label(frame, text="INCORRECT PASSWORD\n\nYou got it wrong!\nA tiny part of you wished that this meant you would die.\nFor real. But reality is often disappointing.\nYou're back at the White Room again.\nJust like every other time.\nDeath just doesn't seem to exist here.",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame31 stuff
# f31_img = PhotoImage(file = "H:\Bugsprayy.png")
# f31_pic_label = Label(frame, image=f31_img)
y30 = tk.Label(frame, text="",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame32 stuff <--
# f32_img = PhotoImage(file = "H:\")
# f32_pic_label = Label(frame, image=f32_img)
y31 = tk.Label(frame, text="",
                 font=("Times New Roman", 18), justify="center", bg="black", fg="white")


# frame33 stuff <-- Safe
f33_img = PhotoImage(file = "H:\Lockett.png")
f33_pic_label = Label(frame, image=f33_img)
y32a = tk.Label(frame, text="//FLASHBACK//\nShe suffered from nightmares, something similar to yours.\nBut she was brave enough to overcome it.\nPerhaps you’re just not strong enough...\nYou remember... She used to say:\n     \"My little bird, I hope when you take that leap\n       of faith, you have nothing to fear anymore...\n//FLASHBACK END//",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")
y32b = tk.Label(frame, text="A leap of faith...\nA leap... a Jump...?!\nIs that what it means?\nMaybe...\nBut you’ve tried jumping off the terrace.\nIt always ends in the White Room.\nWell, It might be different this time.\nYou head straight to the terrace.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame34 stuff <-- Last Terrace
f34_img = PhotoImage(file = "H:\Terracee.png")
f34_pic_label = Label(frame, image=f34_img)
y33 = tk.Label(frame, text="This is it.\nYou take one last look at the stars.\nYou could jump... Or you could head back.\nBut you've exhausted every inch of this nightmare.\nThere is no point in heading back.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white", wraplength=400)


# frame35 stuff <-- Last Terrace(Stay)
# f35_img = PhotoImage(file = "H:\")
# f35_pic_label = Label(frame, image=f35_img)
y34 = tk.Label(frame, text="Alright. No.\nYou don't want to jump. Not right now, at least.\n       ... It doesn't feel like the right decision...\nNevertheless, you leave, but pass out on the way downstairs.\nYou slowly come to yourself.\nYou're in a white room. The White Room.\nYou're back to where you started.\nBut what else did you expect?\nYou're a coward who's afraid to change; to let go.\nYou’re stuck. You can’t get out.\nIt’s a nightmare, and You’re stuck.\nYou’re stuck.\nYou’re stuck. You’re stuck. You’re stuck.\nYou’re stuck. You’re stuck. You’re stuck.\nYou’re stuck. You’re stuck. You’re stuck.\n\nStuck. Stuck. Stuck. Stu—",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# frame36 stuff <-- Last Terrace(Jump)
# f36_img = PhotoImage(file = "H:\")
# f36_pic_label = Label(frame, image=f36_img)
y35 = tk.Label(frame, text="You brace yourself and fall forward.\nYou slowly wake up in a white room.\nSomeone knocks on the door, and a man you recognize walks in.\nHe's from the hospital— not the one in dreams, but the one from reality.\nDoes this mean... you made it out...?\nYou search for your mother's locket on your bedside table.\nIt's there. You see two faces smiling at one another.\nYour mother lives in dreams. You belong here.\nYou’re not sure when you’re going to be okay... but that’s okay.\n\nIt might take a while, but you will make it out of this hospital\nYou won’t get stuck.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")


# frame37 stuff <-- ending 1/2
f37_img = PhotoImage(file = "H:\Endd.png")
f37_pic_label = Label(frame, image=f37_img)
y36 = tk.Label(frame, text="------------------------------\n| ENDING 1/2: CLOSURE |\n------------------------------\nYou made it out. Congratulations!\nIt was the fear of being stuck in a hospital\nthat cursed you into an endless loop of nightmares.\nAfter waking, you realize it might take a while for you to be alright.\nBut you know it’ll happen someday.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# frame38 stuff <-- ending 2/2
f38_img = PhotoImage(file = "H:\Endd (2).png")
f38_pic_label = Label(frame, image=f38_img)
y37 = tk.Label(frame, text="-------------------------------\n| ENDING 2/2: INSANITY |\n-------------------------------\nYou didn't leave.\nYour grief and thoughts weigh you down.\nMaybe things would have been different if you had been braver.",
                 font=("Times New Roman", 16), justify="center", bg="black", fg="white")

# crowbar-picked!
crowbarpick = PhotoImage(file = "H:\Crowbarpickk.png")
crowbarpick_label = Label(frame, image=crowbarpick)

# bugspray picked!
bugspraypick = PhotoImage(file = "H:\Bugsprayy.png")
bugspraypick_label = Label(frame, image=bugspraypick)


# map
fmap_img = PhotoImage(file = "H:\Mapp.png") # Storing the photo in a variable
fmap_pic_label = Label(frame, image=fmap_img) # Converting the variable in to a label and storing it in a new variable


# ------------------------------------------------- Maps ------------------------------------------------------------ #


def map():

    fmap_pic_label.img = fmap_img
    fmap_pic_label.place(x=-10, y=-15)

def map1(): #whiteroom

    m1.place_forget()
    b4.place_forget()
    b4a.place_forget()
    b4b.place_forget()
    b4.place_forget()
    y1.place_forget()
    f4_pic_label.pack_forget()
    map()
    global c1
    c1 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame4)
    c1.place(x=700, y=630)

def map2(): #inspect

    m1.place_forget()
    b4.place_forget()
    back.place_forget()
    y2.place_forget()
    f5_pic_label.pack_forget()
    global c2
    c2 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame5)
    map()
    c2.place(x=700, y=630)

def map3():  # door->corridor

    m1.place_forget()
    b4.place_forget()
    b6a.place_forget()
    b6b.place_forget()
    y3.place_forget()
    f6_pic_label.pack_forget()
    c3 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame6)
    map()
    c3.place(x=700, y=630)


def map4():  # bathroom

    m1.place_forget()
    b4.place_forget()
    b7a.place_forget()
    b7b.place_forget()
    y4.place_forget()
    f7_pic_label.pack_forget()
    c4 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame7)
    map()
    c4.place(x=700, y=630)


def map5():  # inspect knocking

    m1.place_forget()
    b4.place_forget()
    b8a.place_forget()
    b8b.place_forget()
    b8c.place_forget()
    y5.place_forget()
    f8_pic_label.pack_forget()
    c5 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame8)
    map()
    c5.place(x=700, y=630)


def map9a():  # bathroom -> red
    m1.place_forget()
    b4.place_forget()
    b9aa.place_forget()
    y6.place_forget()
    f9a_pic_label.pack_forget()
    c6 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame9a)
    map()
    c6.place(x=700, y=630)


def map9b():  # bathroom -> blue
    m1.place_forget()
    b4.place_forget()
    b7ba.place_forget()
    y7a.place_forget()
    f9b_pic_label.pack_forget()
    c7 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame9b)
    map()
    c7.place(x=700, y=630)


def map9c():  # bathroom -> black
    m1.place_forget()
    b4.place_forget()
    b9ca.place_forget()
    y7b.place_forget()
    f9c_pic_label.pack_forget()
    c7a = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame9c)
    map()
    c7a.place(x=700, y=630)


def map10():  # right -> cafeteria
    m1.place_forget()
    b4.place_forget()
    b10a.place_forget()
    back.place_forget()
    b10b.place_forget()
    y7c.place_forget()
    f10_pic_label.pack_forget()
    c7b = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame10)
    map()
    c7b.place(x=700, y=630)


def map11():  # cafeteria -> inspect
    m1.place_forget()
    b4.place_forget()
    b11a.place_forget()
    back.place_forget()
    y8.place_forget()
    f11_pic_label.pack_forget()
    c7c = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame11)
    map()
    c7c.place(x=700, y=630)


def map12():  # cafeteria -> Death
    m1.place_forget()
    b4.place_forget()
    b12a.place_forget()
    back.place_forget()
    y9.place_forget()
    f11_pic_label.pack_forget()
    c8 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame12)
    map()
    c8.place(x=700, y=630)


def map13():  # staircase

    m1.place_forget()
    b4.place_forget()
    for b13a in frame.winfo_children():
        b13a.place_forget()
    b13b.place_forget()
    for b13c in frame.winfo_children():
        b13c.place_forget()
    back.place_forget()
    y10.place_forget()
    f12_pic_label.pack_forget()
    c9 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame13)
    map()
    c9.place(x=700, y=630)


def map14():  # crowbar show up
    m1.place_forget()
    b4.place_forget()
    b14a.place_forget()
    b14b.place_forget()
    back.place_forget()
    y11.place_forget()
    f13_pic_label.pack_forget()
    c10 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame14)
    map()
    c10.place(x=700, y=630)


def map15():  # terrace
    m1.place_forget()
    b4.place_forget()
    b15a.place_forget()
    back.place_forget()
    b15b.place_forget()
    y12.place_forget()
    f14_pic_label.place_forget()
    c11 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame15)
    map()
    c11.place(x=700, y=630)


def map16():  # jump off terrace
    m1.place_forget()
    b4.place_forget()
    b16a.place_forget()
    back.place_forget()
    y13.place_forget()
    f15_pic_label.place_forget()
    c12 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame16)
    map()
    c12.place(x=700, y=630)


def map17():  # waiting room -> room
    m1.place_forget()
    b4.place_forget()
    b17a.place_forget()
    b17b.place_forget()
    back.place_forget()
    y14.place_forget()
    f16_pic_label.place_forget()
    c13 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame17)
    map()
    c13.place(x=700, y=630)


def map18():  # waiting room
    m1.place_forget()
    b4.place_forget()
    b18a.place_forget()
    b18b.place_forget()
    b18c.place_forget()
    b18d.place_forget()
    back.place_forget()
    y15.place_forget()
    f17_pic_label.place_forget()
    c14 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame18)
    map()
    c14.place(x=700, y=630)


def map19():  # left -> operation area
    m1.place_forget()
    b4.place_forget()
    b19a.place_forget()
    b19b.place_forget()
    back.place_forget()
    y16.place_forget()
    f18_pic_label.place_forget()
    c15 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame19)
    map()
    c15.place(x=700, y=630)


def map20():  # accept offer
    m1.place_forget()
    b4.place_forget()
    b20a.place_forget()
    back.place_forget()
    y17.place_forget()
    f19_pic_label.place_forget()
    c16 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame20)
    map()
    c16.place(x=700, y=630)


def map21():  # OR death w/ crowbar
    m1.place_forget()
    b4.place_forget()
    b21a.place_forget()
    y18.place_forget()
    back.place_forget()
    f20_pic_label.place_forget()
    c17 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame21)
    map()
    c17.place(x=700, y=630)


def map22():  # OR no death w/out crowbar
    m1.place_forget()
    b4.place_forget()
    b22a.place_forget()
    y19.place_forget()
    back.place_forget()
    f21_pic_label.place_forget()
    c18 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame22)
    map()
    c18.place(x=700, y=630)


def map23():  # morgue (right)
    m1.place_forget()
    b4.place_forget()
    b23a.place_forget()
    b23b.place_forget()
    back.place_forget()
    y20.place_forget()
    # f22_pic_label.pack_forget()
    c19 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame23)
    map()
    c19.place(x=700, y=630)


def map24():  # body
    m1.place_forget()
    b4.place_forget()
    b24a.place_forget()
    back.place_forget()
    y21.place_forget()
    # f23_pic_label.pack_forget()
    c20 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame24)
    map()
    c20.place(x=700, y=630)


def map25ha():  # buzzing
    m1.place_forget()
    b4.place_forget()
    b25haa.place_forget()
    b25hab.place_forget()
    back.place_forget()
    y22.place_forget()
    # f24_pic_label.pack_forget()
    c21 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame25ha)
    map()
    c21.place(x=700, y=630)


def map25():  # buzz -> without spray
    m1.place_forget()
    b4.place_forget()
    b25a.place_forget()
    back.place_forget()
    y23.place_forget()
    # f24_pic_label.pack_forget()
    c21 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame25)
    map()
    c21.place(x=700, y=630)


def map26():  # buzz -> with bugspray
    m1.place_forget()
    b4.place_forget()
    b26a.place_forget()
    back.place_forget()
    y24.place_forget()
    # f25_pic_label.pack_forget()
    c22 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame26)
    map()
    c22.place(x=700, y=630)

def map26ha():  # buzz -> with bugspray
    m1.place_forget()
    b4.place_forget()
    b26haa.place_forget()
    back.place_forget()
    y24.place_forget()
    # f25_pic_label.pack_forget()
    c22 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame26ha)
    map()
    c22.place(x=700, y=630)


def map27():
    m1.place_forget()
    b4.place_forget()
    b27a.place_forget()
    back.place_forget()
    y25.place_forget()
    f27_pic_label.place_forget()
    c23 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame27)
    map()
    c23.place(x=700, y=630)


def map28():
    m1.place_forget()
    b4.place_forget()
    entry.place_forget()
    entry1.place_forget()
    y26.place_forget()
    # f28_pic_label.pack_forget()
    c24 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame28)
    map()
    c24.place(x=700, y=630)


def map29():
    m1.place_forget()
    b4.place_forget()
    b28a.place_forget()
    y27.place_forget()
    # f28_pic_label.pack_forget()
    c25 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame29)
    map()
    c25.place(x=700, y=630)


def map30():
    m1.place_forget()
    b4.place_forget()
    b30a.place_forget()
    y28.place_forget()
    # f29_pic_label.pack_forget()
    c26 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame30)
    map()
    c26.place(x=700, y=630)


def map31():
    m1.place_forget()
    b4.place_forget()
    y29.place_forget()
    # f30_pic_label.pack_forget()
    c27 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame31)
    map()
    c27.place(x=700, y=630)


def map32():
    m1.place_forget()
    b4.place_forget()
    y30.place_forget()
    # f31_pic_label.pack_forget()
    c28 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame32)
    map()
    c28.place(x=700, y=630)


def map33a():
    m1.place_forget()
    b4.place_forget()
    y31.place_forget()
    b33a.place_forget()
    # f32_pic_label.pack_forget()
    c29 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame33a)
    map()
    c29.place(x=700, y=630)


def map33b():
    m1.place_forget()
    b4.place_forget()
    b33b.place_forget()
    y31.place_forget()
    b33b.place_forget()
    # f32_pic_label.pack_forget()
    c29 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame33b)
    map()
    c29.place(x=700, y=630)


def map34():
    m1.place_forget()
    b4.place_forget()
    b34a.place_forget()
    b34b.place_forget()
    y32a.place_forget()
    f33_pic_label.pack_forget()
    c30 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame34)
    map()
    c30.place(x=700, y=630)


def map35():
    m1.place_forget()
    b4.place_forget()
    b35a.place_forget()
    y33.place_forget()
    # f34_pic_label.pack_forget()
    c31 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame35)
    map()
    c31.place(x=700, y=630)


def map36():
    m1.place_forget()
    b4.place_forget()
    b36a.place_forget()
    y34.place_forget()
    # f35_pic_label.pack_forget()
    c32 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame36)
    map()
    c32.place(x=700, y=630)


def map37():
    m1.place_forget()
    b4.place_forget()
    y35.place_forget()
    # f36_pic_label.pack_forget()
    c33 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame37)
    map()
    c33.place(x=700, y=630)


def map38():
    m1.place_forget()
    b4.place_forget()
    y36.place_forget()
    # f37_pic_label.pack_forget()
    c34 = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                    command=frame38)
    map()
    c34.place(x=700, y=630)


# -------------------------------------------------- Inventory ------------------------------------------------------ #

def callback1():
    if "crowbar" not in inventory:
        crowbarpick_label.place(x=-5, y=-20)
        global b14a
        global b14b
        bc = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                       command=frame15)
        bc.place(x=700, y=630)
        y11.place_forget()
        b3.place_forget()
        fmap_pic_label.place_forget()
        f14_pic_label.place_forget()
        m1.place_forget()
        b14a.place_forget()
        b14b.place_forget()
        back.place_forget()
        print("You clicked Pick Up")
        inventory.append("crowbar")
        print(inventory)
    else:
        print("You have this")
        pass

def callback2():
    if "bugspray" not in inventory:
        bugspraypick_label.place(x=-20, y=-16)
        global b17a
        global b17b
        bb = tk.Button(frame, text='Close', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                       command=frame18)
        bb.place(x=700, y=630)
        y28.place_forget()
        b3.place_forget()
        fmap_pic_label.place_forget()
        f14_pic_label.place_forget()
        m1.place_forget()
        b17a.place_forget()
        b17b.place_forget()
        back.place_forget()
        print("You clicked Pick Up")
        inventory.append("bugspray")
        print(inventory)
    else:
        print("You have this")
        pass


# -------------------------------------------------Frames------------------------------------------------------------ #



def frame38():

    y33.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c34 in frame.winfo_children():
        c34.place_forget()

    f38_pic_label.img = f5_img
    f38_pic_label.place(x=-2)

    y37.place(x=120, y=150)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map38)
    m1.place(x=15, y=15)
    global b4
    b4.place(x=710, y=630)


def frame37():
    y32a.place_forget()
    y32b.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c33 in frame.winfo_children():
        c33.place_forget()

    f37_pic_label.img = f5_img
    f37_pic_label.place(x=-2)

    y36.place(x=110, y=150)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map37)
    m1.place(x=15, y=15)
    global b4
    b4.place(x=710, y=630)


def frame36():  # --> last terrace jump
    y31.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c32 in frame.winfo_children():
        c32.place_forget()

    # f35_pic_label.img = f5_img
    # f35_pic_label.pack()

    y35.place(x=100, y=150)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map36)
    m1.place(x=15, y=15)
    global b36a
    b36a = tk.Button(frame, text="...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame37)
    b36a.place(x=370, y=630)
    global b4
    b4.place(x=710, y=630)


def frame35(): # --> last terrace stay
    y30.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c31 in frame.winfo_children():
        c31.place_forget()

    # f34_pic_label.img = f5_img
    # f34_pic_label.pack()

    y34.place(x=130, y=150)
    global b35a
    b35a = tk.Button(frame, text="...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame38)
    b35a.place(x=370, y=630)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map35)
    m1.place(x=15, y=15)
    global b4
    b4.place(x=710, y=630)


def frame34(): # Last terrace
    y29.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c30 in frame.winfo_children():
        c30.place_forget()

    f34_pic_label.img = f5_img
    f34_pic_label.place(x=-2)

    y33.place(x=225, y=200)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map34)
    m1.place(x=15, y=15)
    global b34a
    b34a = tk.Button(frame, text="Stay ", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame35)
    b34a.place(x=364, y=360)
    global b34b
    b34b = tk.Button(frame, text="Jump", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame36)
    b34b.place(x=364, y=440)

    global b4
    b4.place(x=710, y=630)


def frame33b(): # Safe Pg2
    y28.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c29 in frame.winfo_children():
        c29.place_forget()

    f33_pic_label.img = f5_img
    f33_pic_label.place(x=-2)

    f33_pic_label.img = f5_img
    f33_pic_label.place(x=-2)

    y32b.place(x=230, y=360)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map33b)
    m1.place(x=15, y=15)

    global b33b

    b33b = tk.Button(frame, text="Terrace", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame34)
    b33b.place(x=350, y=630)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame33a(): # Safe Pg1
    y28.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c28 in frame.winfo_children():
        c28.place_forget()

    f33_pic_label.img = f5_img
    f33_pic_label.place(x=-2)

    y32a.place(x=160, y=360)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map33a)
    m1.place(x=15, y=15)

    global b33a

    b33a = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame33b)
    b33a.place(x=315, y=630)

    global b4
    b4.place(x=710, y=630)


def frame31(): # Try(Entry correct)(In Exit)
    y26.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c27 in frame.winfo_children():
        c27.place_forget()

    #f31_pic_label.img = f5_img
    #f31_pic_label.pack()

    y28.place(x=35, y=150)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map31)
    m1.place(x=15, y=15)

    global b4
    b4.place(x=710, y=630)


def frame30(): # Try(Entry wrong)(In Exit)
    y25.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c26 in frame.winfo_children():
        c26.place_forget()

    # f29_pic_label.img = f5_img
    # f29_pic_label.pack()

    y29.place(x=123, y=200)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map30)
    m1.place(x=15, y=15)

    global b30a

    b30a = tk.Button(frame, text="White Room", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame4)
    b30a.place(x=320, y=630)

    global b4
    b4.place(x=710, y=630)


def frame29(): # Try(Entry correct)(In Exit)
    y24.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c25 in frame.winfo_children():
        c25.place_forget()

    f29_pic_label.img = f5_img
    f29_pic_label.place(x=-2)

    y28.place(x=200, y=360)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map29)
    m1.place(x=15, y=15)

    global b28a

    b28a = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame33a)
    b28a.place(x=315, y=630)

    global b4
    b4.place(x=710, y=630)


def frame28():

    b27a.place_forget()
    back.place_forget()
    b4.place_forget()
    for c24 in frame.winfo_children():
        c24.place_forget()

    f28_pic_label.img = f5_img #<-change the no. to frame no. to avoid confusion
    f28_pic_label.place(x=-2)

    y27.place(x=210, y=360)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map28)
    m1.place(x=15, y=15)

    global entry
    entry = tk.Entry(frame, bg="white", font=("Times New Roman", 20), border=2)
    entry.place(x=178, y=500)

    def password():
        if entry.get() == 'bird':
            frame29()
        else:
            frame30()

    global entry1
    entry1 = tk.Button(frame, text="Enter", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                       command=password)
    entry1.place(x=508, y=491)

    b4.place(x=710, y=630)


def frame27(): # Exit
    y22.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c23 in frame.winfo_children():
        c23.place_forget()

    f27_pic_label.img = f5_img
    f27_pic_label.place(x=-2)

    y26.place(x=105, y=350)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map27)
    m1.place(x=15, y=15)
    global b27a
    global back
    b27a = tk.Button(frame, text="Try ", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame28)
    b27a.place(x=354, y=500)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame18)
    back.place(x=20, y=630)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)

def frame26ha():  # buzz -> without bugspray

    y19.place_forget()
    b3.place_forget()
    f3_pic_label.pack_forget()
    for c22 in frame.winfo_children():
        c22.place_forget()

    f26ha_pic_label.img = f5_img
    f26ha_pic_label.place(x=-2)

    y25.place(x=110, y=405)

    global b26haa
    global back

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map26ha)
    m1.place(x=15, y=15)

    b26haa = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                       command=frame4)
    b26haa.place(x=310, y=630)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame26(): # buzz -> with bugspray
    y21.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c22 in frame.winfo_children():
        c22.place_forget()

    f26_pic_label.img = f5_img
    f26_pic_label.place(x=-20, y=-20)

    y24.place(x=80, y=340)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map26)
    m1.place(x=15, y=15)
    global b26a
    b26a = tk.Button(frame, text="Waiting Area", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame18)
    b26a.place(x=300, y=630)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame25(): # buzz -> without bugspray

    y19.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c21 in frame.winfo_children():
        c21.place_forget()

    f25_pic_label.img = f5_img
    f25_pic_label.place(x=-2)

    y23.place(x=110, y=405)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map25)
    m1.place(x=15, y=15)
    global b25a
    b25a = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame4)
    b25a.place(x=310, y=630)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2, command=root.destroy)
    b4.place(x=710, y=630)


def frame25ha(): # buzzing
    y20.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c21 in frame.winfo_children():
        c21.place_forget()

    f25ha_pic_label.img = f5_img
    f25ha_pic_label.place(x=-20, y=-20)

    y22.place(x=205, y=150)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map25ha)
    m1.place(x=15, y=15)
    global b25haa
    global b25hab
    if "bugspray" in inventory:
        b25haa = tk.Button(frame, text="Run!", bg="black", fg="white", font=("Times New Roman", 17), border=2,
                         command=frame20)
        b25haa.place(x=280, y=480)

        b25hab = tk.Button(frame, text="Use Bugspray", bg="black", fg="white", font=("Times New Roman", 17), border=2,
                         command=frame26)
        b25hab.place(x=400, y=480)
    else:
        b25haa = tk.Button(frame, text="Run!", bg="black", fg="white", font=("Times New Roman", 17), border=2,
                         command=frame20)
        b25haa.place(x=280, y=480)

        b25hab = tk.Button(frame, text="Use Bugspray", bg="black", fg="white", font=("Times New Roman", 17), border=2,
                         command=frame25)
        b25hab.place(x=400, y=480)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame24(): # body

    y19.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c20 in frame.winfo_children():
        c20.place_forget()

    f24_pic_label.img = f5_img
    f24_pic_label.place(x=-20, y=-20)

    y21.place(x=115, y=425)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map24)
    m1.place(x=15, y=15)
    global b24a
    b24a = tk.Button(frame, text="Waiting Area", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame18)
    b24a.place(x=310, y=630)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2, command=root.destroy)
    b4.place(x=710, y=630)

def frame23(): # morgue (right)
    y18.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c19 in frame.winfo_children():
        c19.place_forget()

    f23_pic_label.img = f5_img
    f23_pic_label.place(x=-2, y=-2)

    y20.place(x=35, y=100)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map23)
    m1.place(x=15, y=15)
    global b23a
    global b23b
    global back
    b23a = tk.Button(frame, text="Body", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame24)
    b23a.place(x=605, y=115)

    b23b = tk.Button(frame, text="Buzzing", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame25ha)
    b23b.place(x=590, y=215)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame18)
    back.place(x=20, y=630)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame22(): # OR death w/out crowbar
    y17.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()
    for c18 in frame.winfo_children():
        c18.place_forget()

    f22_pic_label.img = f5_img
    f22_pic_label.place(x=-2, y=-2)

    y19.place(x=110, y=390)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map22)
    m1.place(x=15, y=15)
    global b22a
    b22a = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame4)
    b22a.place(x=310, y=570)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame21(): # OR no death w/ crowbar
    y16.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f19_pic_label.pack_forget()
    for c17 in frame.winfo_children():
        c17.place_forget()

    f21_pic_label.img = f5_img
    f21_pic_label.place(x=-2)

    y18.place(x=150, y=390)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map21)
    m1.place(x=15, y=15)
    global b21a
    b21a = tk.Button(frame, text="Waiting Area", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame18)
    b21a.place(x=310, y=570)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame20(): # accept offer
    y16.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f19_pic_label.place_forget()
    for c16 in frame.winfo_children():
        c16.place_forget()

    f20_pic_label.img = f5_img
    f20_pic_label.place(x=-10, y=-2)

    y17.place(x=56, y=420)
    global b20a
    b20a = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame4)
    b20a.place(x=310, y=630)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map20)
    m1.place(x=15, y=15)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame19(): # left -> operation area
    y15.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f18_pic_label.pack_forget()
    for c15 in frame.winfo_children():
        c15.place_forget()

    f19_pic_label.img = f5_img
    f19_pic_label.place(x=-5, y=-2)

    y16.place(x=300, y=70)
    global b19a
    global b19b
    global back
    if "crowbar" in inventory:
        b19a = tk.Button(frame, text="Accept Offer", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                         command=frame20)
        b19a.place(x=470, y=350)

        b19b = tk.Button(frame, text="Escape By Fighting", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                         command=frame21)
        b19b.place(x=430, y=450)
    else:
        b19a = tk.Button(frame, text="Accept Offer", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                         command=frame20)
        b19a.place(x=470, y=350)

        b19b = tk.Button(frame, text="Escape By Fighting", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                         command=frame22)
        b19b.place(x=430, y=450)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map19)
    m1.place(x=15, y=15)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame18)
    back.place(x=20, y=630)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame18(): # waiting area
    y18.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f21_pic_label.place_forget()
    f17_pic_label.place_forget()
    y10.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f13_pic_label.pack_forget()
    for c14 in frame.winfo_children():
        c14.place_forget()

    f18_pic_label.img = f5_img
    f18_pic_label.place(x=-5, y=-2)

    y15.place(x=110, y=150)
    global b18a
    global b18b
    global b18c
    global b18d
    global back
    b18a = tk.Button(frame, text="Left", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame19)
    b18a.place(x=150, y=370)

    b18b = tk.Button(frame, text="Right", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame23)
    b18b.place(x=280, y=370)

    if "bugspray" not in inventory:
        b18c = tk.Button(frame, text="Inspect", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                         command=frame17)
        b18c.place(x=420, y=370)
    else:
        b18c = tk.Button(frame, text="(Done)", bg="black", fg="white", font=("Times New Roman", 20), border=2)
        b18c.place(x=420, y=370)


    b18d = tk.Button(frame, text="Exit", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame27)
    b18d.place(x=580, y=370)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map18)
    m1.place(x=15, y=15)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame13)
    back.place(x=20, y=630)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame17(): # waiting area -> inspect
    global b17a
    global b17b
    global m1
    global back
    y18.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f15_pic_label.place_forget()
    y13.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f16_pic_label.place_forget()
    y18.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f21_pic_label.pack_forget()
    for c13 in frame.winfo_children():
        c13.place_forget()

    f17_pic_label.img = f5_img
    f17_pic_label.place(x=-2)

    y14.place(x=140, y=500)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map17)
    m1.place(x=15, y=15)

    b17a = tk.Button(frame, text="Pick Up", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=callback2)
    b17a.place(x=500, y=500)

    b17b = tk.Button(frame, text="Leave It", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame18)
    b17b.place(x=500, y=585)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame18)
    back.place(x=20, y=630)



def frame16(): # jump off terrace
    f13_pic_label.pack_forget()
    y12.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f15_pic_label.place_forget()
    for c12 in frame.winfo_children():
        c12.place_forget()

    f16_pic_label.img = f5_img
    f16_pic_label.place(x=-2, y=-2)

    y13.place(x=190, y=380)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map16)
    m1.place(x=15, y=15)
    global b16a
    b16a = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame4)
    b16a.place(x=310, y=570)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)



def frame15(): # terrace
    y11.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f14_pic_label.pack_forget()
    for c11 in frame.winfo_children():
        c11.place_forget()

    f15_pic_label.img = f5_img
    f15_pic_label.place(x=-10, y=-10)

    y12.place(x=216, y=200)
    global b15a
    global b15b
    b15a = tk.Button(frame, text="Back", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame13)
    b15a.place(x=356, y=340)

    b15b = tk.Button(frame, text="Jump", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame16)
    b15b.place(x=356, y=420)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map15)
    m1.place(x=15, y=15)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame14(): # crowbar show up
    global m1
    y10.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f13_pic_label.pack_forget()
    for c10 in frame.winfo_children():
        c10.place_forget()

    f14_pic_label.img = f5_img
    f14_pic_label.place(x=-2)

    y11.place(x=500, y=200)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map14)
    m1.place(x=15, y=15)
    global b14a
    global b14b
    global back
    b14a = tk.Button(frame, text="Pick Up", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=callback1)
    b14a.place(x=580, y=300)

    b14b = tk.Button(frame, text="Leave It", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame15)
    b14b.place(x=580, y=370)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame13)
    back.place(x=20, y=630)



def frame13(): # staircase
    y9.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f12_pic_label.pack_forget()
    y8.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f11_pic_label.pack_forget()
    y3.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f6_pic_label.pack_forget()
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f9c_pic_label.pack_forget()
    f10_pic_label.pack_forget()
    for c9 in frame.winfo_children():
        c9.place_forget()

    f13_pic_label.img = f5_img
    f13_pic_label.pack()

    y10.place(x=270, y=100)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map13)
    global b13a
    global b13b
    global b13c
    global back
    if "crowbar" not in inventory:
        b13a = tk.Button(frame, text="Up", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame14)
        b13a.place(x=430, y=220)
    else:
        b13c = tk.Button(frame, text="Up", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame15)
        b13c.place(x=430, y=220)

    b13b = tk.Button(frame, text="Down", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame18)
    b13b.place(x=300, y=220)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame10)
    back.place(x=20, y=630)

    m1.place(x=15, y=15)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)

    b4.place(x=710, y=630)


def frame12(): # cafeteria -> death
    y8.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f11_pic_label.pack_forget()
    for c8 in frame.winfo_children():
        c8.place_forget()

    f12_pic_label.img = f5_img
    f12_pic_label.place(x=-2)

    y9.place(x=160, y=400)
    global b12a
    b12a = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame4)
    b12a.place(x=310, y=570)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map12)
    m1.place(x=15, y=15)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)

def frame11(): # cafeteria -> inspect
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f10_pic_label.pack_forget()
    for c7c in frame.winfo_children():
        c7c.place_forget()

    f11_pic_label.img = f5_img
    f11_pic_label.pack()

    y8.place(x=50, y=250)
    global b11a
    global back
    b11a = tk.Button(frame, text='Eat Organs!', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame12)
    b11a.place(x=200, y=550)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame10)
    back.place(x=450, y=550)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map11)
    m1.place(x=15, y=15)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)

def frame10(): # right -> cafeteria
    y8.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f11_pic_label.pack_forget()
    y3.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f6_pic_label.pack_forget()
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f9c_pic_label.pack_forget()
    y10.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f13_pic_label.pack_forget()
    for c7b in frame.winfo_children():
        c7b.place_forget()

    f10_pic_label.img = f5_img
    f10_pic_label.pack()

    y7c.place(x=260, y=500)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map10)
    m1.place(x=15, y=15)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)

    global b10a
    global b10b
    global back

    b10a = tk.Button(frame, text='Staircase', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame13)
    b10a.place(x=255, y=630)

    b10b = tk.Button(frame, text='Inspect', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame11)
    b10b.place(x=430, y=630)

    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                     command=frame6)
    back.place(x=20, y=630)

def frame9c(): # bathroom -> black
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f9b_pic_label.pack_forget()
    for c7a in frame.winfo_children():
        c7a.place_forget()

    f9c_pic_label.img = f5_img
    f9c_pic_label.place(x=-2)

    y7b.place(x=30, y=300)
    global b9ca
    global b4
    b9ca = tk.Button(frame, text="Corridor", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame6)
    b9ca.place(x=330, y=520)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map9c)
    m1.place(x=15, y=15)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)

def frame9b(): # bathroom -> blue
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f9a_pic_label.pack_forget()
    for c7 in frame.winfo_children():
        c7.place_forget()

    f9b_pic_label.img = f5_img
    f9b_pic_label.place(x=-2)

    y7a.place(x=70, y=400)
    global b7ba
    global b4
    b7ba = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                     command=frame4)
    b7ba.place(x=310, y=570)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map9b)
    m1.place(x=15, y=15)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame9a(): # bathrooom -> red
    y5.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f8_pic_label.pack_forget()
    for c6 in frame.winfo_children():
        c6.place_forget()

    f9a_pic_label.img = f5_img
    f9a_pic_label.place(x=-2)

    y6.place(x=80, y=400)
    global b9aa
    global b4
    b9aa = tk.Button(frame, text="Continue...", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame4)
    b9aa.place(x=310, y=570)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map9a)
    m1.place(x=15, y=15)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame8(): # inspect knocking
    y4.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f7_pic_label.pack_forget()
    for c5 in frame.winfo_children():
        c5.place_forget()

    f8_pic_label.img = f5_img
    f8_pic_label.place(x=-2)

    y5.place(x=80, y=400)
    global b8a
    global b8b
    global b8c
    global b4
    b8a = tk.Button(frame, text="Red", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                    command=frame9a)
    b8a.place(x=100, y=550)

    b8b = tk.Button(frame, text="Blue", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame9b)
    b8b.place(x=365, y=550)

    b8c = tk.Button(frame, text="Black(?)", bg="black", fg="white", font=("Times New Roman", 20), border=2,
                    command=frame9c)
    b8c.place(x=590, y=550)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map5)
    m1.place(x=15, y=15)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame7(): # bathroom
    y3.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f6_pic_label.pack_forget()
    for c4 in frame.winfo_children():
        c4.place_forget()

    f7_pic_label.img = f5_img
    f7_pic_label.place(x=-2)

    y4.place(x=80, y=400)
    global b7a
    global b7b
    global b4
    b7a = tk.Button(frame, text="Inspect Knocking", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame8)
    b7a.place(x=200, y=550)

    b7b = tk.Button(frame, text="Back", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame6)
    b7b.place(x=450, y=550)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map4)
    m1.place(x=15, y=15)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)


def frame6(): #door-> corridor
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f10_pic_label.pack_forget()
    y4.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f7_pic_label.place_forget()
    y2.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f5_pic_label.place_forget()
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f9c_pic_label.pack_forget()
    for c3 in frame.winfo_children():
        c3.place_forget()

    f6_pic_label.img = f5_img
    f6_pic_label.place(x=-2)

    y3.place(x=250, y=370)
    global b6a
    global b6b
    global b4
    b6a = tk.Button(frame, text="Left", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame7)
    b6a.place(x=255, y=550)

    b6b = tk.Button(frame, text="Right", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame10)
    b6b.place(x=450, y=550)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map3)
    m1.place(x=15, y=15)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)



def frame5(): #inspect in white room


    y1.place_forget()
    f4_pic_label.pack_forget()
    for c2 in frame.winfo_children():
        c2.place_forget()

    f5_pic_label.img = f5_img
    f5_pic_label.place(x=90, y=90)

    y2.place(x=83, y=250)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map2)
    m1.place(x=15, y=15)
    global b4
    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=root.destroy)
    b4.place(x=710, y=630)
    global back
    back = tk.Button(frame, text='Back', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=frame4)
    back.place(x=20, y=630)


def frame4(): #whiteroom

    global m1   # This is used when you are defining a variable in the def function but using it outside the def function. It technically becomes universal
    f25_pic_label.pack_forget()
    y13.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f16_pic_label.pack_forget()
    y19.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f22_pic_label.place_forget()
    y8.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f12_pic_label.pack_forget()
    y3.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f6_pic_label.pack_forget()
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f9b_pic_label.pack_forget()
    y6.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f9a_pic_label.place_forget()
    f17_pic_label.pack_forget()
    y.place_forget()
    b3.place_forget()
    fmap_pic_label.place_forget()
    f3_pic_label.pack_forget()

    inventory.clear()
    print(inventory)

    for c1 in frame.winfo_children(): # This rarely works, but frame.winfo_children considers all the widgets in the frame, e.g. button, label, etc.
        c1.place_forget()

    f4_pic_label.img = f4_img
    f4_pic_label.place(x=-2)

    y1.place(x=185, y=370)

    global b4a
    global b4b
    global b4

    b4a = tk.Button(frame, text="Inspect", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame5)
    b4a.place(x=235, y=500)

    b4b = tk.Button(frame, text="Door", bg="black", fg="white", font=("Times New Roman", 20), border=2, command=frame6)
    b4b.place(x=455, y=500)

    m1 = tk.Button(frame, text='Map', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                   command=map1)
    m1.place(x=15, y=15)

    b4 = tk.Button(frame, text='Quit', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2, command=root.destroy)
    b4.place(x=710, y=630)



def frame3(): #intro

    global b3
    g.destroy()
    #f2_pic_label.destroy()
    f3_pic_label.img = f3_img
    f3_pic_label.place(x=-2)
    y.place(x=220, y=340)

    b3 = tk.Button(frame, text='Next', bg='black', fg='white', font=('Times New Roman', 20, 'bold'), border=2,
                  command=frame4)
    b3.place(relx=0.45, rely=0.86)


def frame2(): #loading

    b2.destroy()
    f1_pic_label.destroy()
    w.destroy()
    r.destroy()

    g.place(relx=0.3, rely=0.45)

    #f2_pic_label.img = f2_img
    #f2_pic_label.place(x=-10, y=90)

    root.after(2000, frame3)


def frame1(): #welcome

    global b2
    b1.destroy()
    photo_label.destroy()
    exit_button.destroy()
    w.place(relx=0.275, rely=0.09)
    r.place(relx=0.3, rely=0.65)

    f1_pic_label.img = f1_img  # to keep the reference for the image.
    f1_pic_label.place(x=135,y=160)  # <--- pack

    b2 = tk.Button(frame, text='Continue', bg='black', fg='white', font=('Times', 16, 'bold'), border=3, command=frame2)
    b2.place(relx=0.44, rely=0.79)

#lucid dreams frame
b1 = tk.Button(frame, text='START', bg='black', fg='white', font=('Courier', 18, 'bold'), border=3, command=frame1)
b1.place(relx=0.439, rely=0.60) # It's out of the def function, hence is the first most button that appears, the click button

exit_button = tk.Button(frame, text='QUIT', bg='black', fg='white', font=('Courier', 18, 'bold'), border=3, command=root.destroy)
exit_button.place(relx=0.448, rely=0.70)


root.mainloop() # Last thing that should exist, the excution function
