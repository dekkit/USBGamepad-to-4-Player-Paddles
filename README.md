# USBGamepad-to-4-Player-Paddles
A straightforward padhack to convert 1 x standard usb gamepad into 4 x paddles for playing your favorite retro paddle games that support up to 4 players.    


## Introduction
While exploring the list of games that make use of the paddle controller, I came across Atari's Warlords arcade game (https://en.wikipedia.org/wiki/Warlords_(1980_video_game) which included support for up 4 players using paddles.   I was keen to see if I could cheaply make a 4 player set of paddles version using a single PCB from a modern gamepad.

The original Paddle controllers used on Atari 2600 / C64 and older arcade games are fairly basic, typically using just a potentiometer (1M Ohm for an Atari) and a few wires to connect microswitches for buttons.   My experience on converting them to use on modern PCs is a bit mixed (they sort of work ok but not that well) - other experiences found online suggest similar.

![image](https://github.com/user-attachments/assets/f275eff4-ab17-409e-a38b-a51df1fd880c)
![image](https://github.com/user-attachments/assets/28b7070e-184c-4c70-a7d6-4d0b61cfb6fd)

Most modern USB gamepads have two analog thumbsticks, which operate very similar to how the original paddles work.
They are really just very small sets of 10k (typically) potentiometers.    

This is an example of a cheap clone x360 usb gamepad with 2 x analog thumbsticks.

![gamepad](https://github.com/user-attachments/assets/7812755b-dbbf-46f4-8c40-d8dd1fe98534)


This project's goal was to remove the smaller 10k pots on the gamepad PCB and replace them with external ones plus remap the buttons so that each player gets 2 x buttons each.

While this project requires no coding / programming skills, as with all padhacks, you will need basic soldering skills.


### Parts List
- 4 x 10k Pots (Linear B)
- 4 x Dial / Knob Covers for Pot (check to make sure they are compatible with your Pot shaft type) 
- 8 x 30mm Buttons (arcade style, 2 x for each player)
- 2 x 24mm Buttons (arcade style, 2 x for coin / start - only for first player) 
- Wires / Dupont Wires (depending if you want to make it socketed or not)
- Arcade button wiring (if you are planning to use arcade style buttons / microswitches)
- 4 x Boxes / cases to mount the paddles in and buttons (I used cheap wooden craft boxes)
- Something to drill button holes (Step drill bit works great - these are a cone shaped drill bit)
- 3 x DB9 female sockets (optional - depending how you want to connect the other players to the usb gamepad pcb)
- 3 x DB9 cables (optional - depending on how you want to connect other players to usb game pcb) 


### USB Gamepad PCB
Stripe the gamepad down to the PCB (remove any rumble motors)

![image](https://github.com/user-attachments/assets/a1310436-6ceb-4a4d-8d7d-5c231bb7f174)

Example of the 10k Pots (in black, you will see 2 on each thumbstick)

![image](https://github.com/user-attachments/assets/f925e5f3-0545-440f-a778-bde97b992f13)


Remove Thumbstick Pots (and any microswitches)
![image](https://github.com/user-attachments/assets/41e85c84-15d2-49db-8a52-da2072fe394f)


Take note of the pins for each of the 4 x POTS  (highlighted in yellow on this PCB)
![image](https://github.com/user-attachments/assets/878bf533-9596-4c44-b412-a75ac3f0393a)

Back + Start + 8 x Buttons (highlighted in red on this PCB)

Note: Genuine XBOX 360 controllers have a number test points (TP) that area easier to solder to - google for more information. 


### Solder Wires to PCB
I went with a bunch of dupont cables to make it easy to test and reconfigure
![image](https://github.com/user-attachments/assets/e13870c4-4bc2-4669-b48b-59eba8b49e52)


In this example - I've soldered dupont wires directly to the button contacts and created a breakout adapter to assist in testing/rewiring (optional).

![image](https://github.com/user-attachments/assets/6c7ffbcd-4ec4-47fe-ad96-d3bcd6285366)

### Layout
Each player is connected to player 1 via DB9 cables:

![image](https://github.com/user-attachments/assets/b6fe9b1b-d080-4eba-9c23-1b4083666936)


### PCB Wiring Reference
I've used color to denote the wiring for each player.  Note the Gamepad PBC is hosted within the player 1 box and why it is not mapped to a DB9 socket.

![image](https://github.com/user-attachments/assets/c14e3714-6d4b-421a-a293-dc0b4c8d5513)

4 Pin IDC (not pictured but used to connect Back / Start buttons)

![image](https://github.com/user-attachments/assets/fffe3336-5711-4a61-a5b4-2859a554a996)


### PCB to DB9 Wiring Reference (repeat for each extra player)
The following was used to connect the USB gamepad to  players 2, 3, and 4:
![image](https://github.com/user-attachments/assets/1bd42633-72ac-45e6-b006-800ea3996e76)

Note: Test the wire color is correct for the pin if you are buying cables of online stores.

![image](https://github.com/user-attachments/assets/698fc31b-3f8f-4131-9120-c6c1972bfd39)




### Internal Wiring Examples
**Player 1** 

Contains USB gamepad PCB, breakout PCB which is wired to POT / Buttons and  3 x DB9 female sockets connected to the back of the box.
![image](https://github.com/user-attachments/assets/8df0316b-44b8-4eb6-8eeb-79459e532359)

Example of 3 x DB9 sockets (connecting the other players)

![image](https://github.com/user-attachments/assets/082f370c-e72d-4b1e-a855-90718c46cbdb)


**Players 2,3,4**

Each connected to main unit with via cable with a DB9 male socket.
![image](https://github.com/user-attachments/assets/d6c8fcea-5841-4456-88b1-43a8c9c55da2)


**Almost finished - the set of 4**

Using cheap wooden craft boxes, this is close to how the prototype looked.   While looking very very DIY, they do play quite well on given how low cost the overall project is.   

![image](https://github.com/user-attachments/assets/bf06488a-c50a-4c89-a1a8-07d9a5809f51)


### Final words...
Atari's Warlords is actually really fun to play with 3-4 players.   Highly recommended!
