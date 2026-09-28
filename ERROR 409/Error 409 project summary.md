# tl;dr

**What**
A portable, two-player phygital game that teaches binary-to-decimal conversion through conflict on a shared device, later extended into a remote digital game.

**Why**
Binary conversion can be difficult to learn, while existing educational games often focus on solving puzzles quickly or competing against a computer. Error 409 was designed to make learning more engaging by using direct player conflict, challenge, and meaningful  interaction and game design to make the process more engaging and fun.

**My role**
Contributed to the research, prototyping, iterative gameplay development, interaction design, and the transition from the phygital prototype to the digital version.

**Result**
Error 409 evolved from an iterative game concept into a portable educational game prototype, was published at CHI PLAY Companion ’24, and was later digitized as a playable browser game on [Chamka Labs](https://www.chamkalabs.com/error409).

# Context
Error 409 began as an exploration into making binary-to-decimal conversion more engaging. After reviewing existing educational games, we experimented with competition and conflict as core mechanics, iterating from larger game boards to a compact two-player experience. The concept then evolved into a phygital game with a shared console, physical switches, and a digital display, before being extended into a playable browser-based version.

# Design, Playtest, Iterate!
### Iteration #1 & #2
![[Pasted image 20260921221100.png]]
- The first version used a large 5×10 or 8×10 grid. Players secretly selected three numbers and took turns placing 1s to form their target numbers in binary. However, the setup took too long and the large grid limited strategic interaction, leading to a more compact design.
- The second version used a smaller 5×5 or 8×8 grid, where players placed 0s and 1s to form their secret numbers in binary. While this created competition, it lacked direct conflict, and players often focused on blocking each other instead of completing their own numbers.

### Iteration #3
![[Pasted image 20260921222001.png]]
The third version introduced a single row with eight binary slots. Players took turns flipping 0/1 chips to form their secret numbers, creating direct conflict and competition. User testing showed the concept was engaging, but players could choose overly simple numbers, leading to randomized numbers in the final design.

### Iteration #4
![[Pasted image 20260921222139.png]]
In this iteration we wanted to continue most features from the 3rd iteration and build upon it, we transformed the game into a portable phygital console with eight physical switches, a digital display, and a claim button thereby giving the game a new medium to play it and unlocking us with the powers of the programming in a simple game like this. Players received randomly assigned secret numbers and competed by switching bits to recreate them in binary, combining physical interaction with digital feedback.

## Developing the phygital version
![[Pasted image 20260927150643.png]]

Yash and Anumeha worked on the modelling and 3D printing part of the device, while I worked on programming the raspberry pi pico to work with switches and display the output on the E-ink display, and also wrote the logic for the gameplay.
We also decided to make the game completely portable, so I made it work with a battery as well as direct USB connection to a charging point.
A simple E-ink display was chosen as it shows only 2 colours, Black and white and goes well with the binary theme, Also it is highly energy efficient and only uses energy to show any change in the display and it doesn't need to be separately powered off.
> Video of the game for more details

Try the game in the emulator
> Interactive Emulator of the game 

## We were selected for CHI Play 2024 for Demoing our game
> Link of the paper
> Some photos of the Finland conference

and we won the most polished gameplay award as well 🥳

# Phase 2
We now also wanted to make this game playable remotely by interested players.
Hence we started creating a website version of the game, but we did not want to make an emulated version of the original game, and rather enrich it with new features which would be available with this medium.

I made use of web sockets to let people create and join game rooms and alow them to play the game remotely with either random strangers or with sharing private links to play with friends.

We made the game mobile first, added web-haptics and sounds to enhance interactions.
We later also added time limits to games to add time pressure in these games and make them more fun and engaging.

We asked for feedback on finishing or quitting the game and also track gameplay and analytics for the game and have improved it using that data as well.

> website link here and a motion designed gameplay.

# Reflection
We created multiple iterations of the game, playtesting the lowest-fidelity versions as early as possible to validate the core idea. Once the fundamental gameplay was established, we explored different mediums and used the unique qualities of each to introduce new features and improve the experience. Through repeated testing and refinement, we created a simpler and more engaging game. This project taught me that strong game experiences emerge through experimentation and iteration rather than from a single final idea.