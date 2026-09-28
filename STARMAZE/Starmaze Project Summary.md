# tl;dr
**What**
Star Maze is an asymmetric two-player VR experience connecting a VR maze runner with a real-time mobile application to control the maze.

**Why**
To explore shared virtual spaces, asymmetric game design and interaction in virtual reality medium.

**My role**
Contributed to the interaction design, prototyping, and playtesting of the VR and mobile experience.

**Result**
A repeatable outreach game that won the Best Project Award at India HCI 2024 and was selected to be presented at Laval Virtual 2025.

# Context
This was a college project for which we were given 3 weeks to explore Virtual reality as a medium and the interactions which we could possibly design within it, we decided to explore all of this while building a game.

# Concept
Star Maze is an asymmetric competitive experience built on the contrast between embodiment and control. One player, the Traveller, is physically immersed in a VR maze, experiencing urgency and spatial uncertainty. The other, the Guradian, uses a mobile device to view the entire map and manipulate the environment from a distance.
Inspired by Among us and other similar asymmetric games, we wanted to make a competitive asymmetric game, which would also be on two different platforms letting both players experience 2 different views of the same game having completely different abilities and opposite goals. We also wanted to focus on the replay-ability aspect of the game. We kept the entire gameplay within a 3 minute time limit.

# Gameplay and roles
> can be designed as 2 cards side by side


 ![[Layer 1.png|271]]![[Layer 2.png|188]]
**Player 1 : VR Player (The Travellers)**
Objective: Navigate through the maze and reach the end destination, marked by a focused light, before time runs out.

**Player 2: Mobile Player (The Guardian)**
Objective: Use strategic abilities to prevent the VR player from reaching the end destination within the time limit.

# Visualising the concept
We started storyboarding to visualise the concept and ideas before investing time in prototyping.

-----
Add storyboarding stuff

------

# Initial prototype
To test out interactions and explore locomotion of a player within the VR game, multiple methods of locomotion were explored and 2 types of locomotion methods were chosen at the end to be built each having their own pros and cons 
Locomotion techniques finalised
1. Controller/stick driven movement
2. In place walking/running (tracked using head movement)

> attach video of the initial prototype and exploration of locomotion techniques

# Exploring visual design for the game
> Some images of explorations

# Balancing powers
## Powers given to the traveller
![[VR view.png]]
The traveller could get trapped by the guardian in such cases traveller should have some powers to realistically accomplish their goal.
1. Punch walls to break through them
2. Double clap to teleport to a random place.
3. Traveller would be able to view the map so that they can figure out the fastest possible route for them to complete the maze

## Powers given to the guardian
![[mobile UI.png]]
1. Guardian would be able to view the position of the traveller every 5 seconds
2. Guardian could rotate as many rotatable walls as possible.
3. Guardian can view the location of the traveller when they teleport.
4. There are landmines laid on the maze floor randomly, and when a traveller steps on one of them, they expose their location and also get slowed down.

# Final prototype
The VR and mobile application were connected using web sockets to establish low latency/lag gameplay and data from the games was stored in postgres databases using Supabase.

https://www.youtube.com/watch?v=tt2D6jd4IVA

# We didn't stop here
We exhibited the prototype in our college to our peers performed playtesting and gathered feedback.
- Even after providing above stated power ups to the guardian, traveller was highly overpowered and the game still felt unbalanced. To resolve this we did not change any powerups of any player as that would have overloaded the players, rather we added a leaderboard for the guardian, to let them know how well of a guardian role were they able to play.
![[Leaderboard img.png]]
- In-place walking and running, tracked through hand movement, were introduced to reduce reliance on head movements for locomotion. Using natural arm-swinging gestures made movement more intuitive, accessible, and less physically tiring.
- Closing of virtual eyelids during the teleportation power-up usage was added to reduce motion sickness.
- In future versions, we would add a wall-breaking animation to provide clearer, more immediate feedback when the Traveller breaks through a wall.
# And we won!!
> Image for winning India HCI 2024 and presented at Laval virtual 2025 

# Reflection
Star Maze functions as both an interactive game and a demonstrator for VR based interaction design, it helps audiences understand concepts such as immersive environments, asymmetric multiplayer systems, and cross device interaction. The short session length allows many participants to experience the system within a limited time window. The clear spectator value supports engagement even for those not directly playing, making it effective for public demonstrations. 

### Some lessons we learned along the way
1. Before jumping into Unity/Unreal, one must try role-playing (Body storming) interactions in real life.
2. Scope Wisely – Time constraints force clear prioritization of features.
3. User Testing is Key – Even in a short timeline, playtesting revealed crucial insights.
4. Having a strong team with people from diverse backgrounds for such dense projects is extremely crucial.


