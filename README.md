# Jason Kardon IMGD4000 Development Portfolio
Chord Clash
Role: Programmer, Audio Implementer, Designer
Tools Used: Unreal Engine 5, GitHub
Language: Blueprints
Genre: PvP Ryhthm Game

Game Description:
Chord Clash is a PvP baed ryhthm game where you are fighting with your opponent to do the best in your song.
The more accurate you are with your notes, the more damage you will do.

Contributions:
- Developed powerup system
    - Created Algorithm for giving players powerups based upon the difference in their health
    - Created system for physcially spawning powerups and using them
    - Implemented fully 3 powerups and helped implement the 3 others
- Implemented a total of 21 different sounds
- Implemented in game hud to display relevant information such as health and combo count while the game is running
- Created particles for taking damage and healing
- Implemented animations for both Beat Head and Bunny Girl and wrote the logic for triggering them
- Numerous bug fixes and quality of life changes

Challenges:
- One of the first major challenges I faced was learning Unreal and blueprints as I had never used them before. It took some time for me to start understanding how blueprints work and what the important nodes were. I overcame this challenge by watching many tutorials on the inner workings of Unreal and the basics of blueprints.
- A major challenge that we faced was fixing an issue with the animations where it would freeze if you pressed the key in rapid succession. We got everyone on the team together and put our heads together in order to try and find a fix. After much trial and error, we fixed it by setting the animations to loop and modifying the way the key presses were setting the variables.
- Another challenge I faced was when I didn't pull fully from main after creating a branch in order the make the credits page, so there were merge conflicts with the menu blueprint and I thought that I would have to redo the entire credits page. I got around this by copying all the widgets of the credits page to another ui blueprint that was not being touched, pulling from main and then copying it back into the main menu blueprint. This saved the few hours of work it would've take me to redo the page.

Code Architecture:
- One of my major jobs was to implement the powerups system. I first created a base powerup class and then created 6 children classes for each of the 6 powerups. I did this so I could have the player blueprint store a variable containing their current powerup. I created a powerup spawner class which handles all of the logic for the powerups: determining which powerup to give and actually assigning them to the player
- The animation state machine starts in the idle pose. Whenever a key is pressed, it goes to the corresponding animation. It returns back to idle was it recieves a notify that the animation is finished.
![image](https://github.com/jtkardon/imgd4000-development-portfolio/assets/93606493/2c5c84ec-2b32-43aa-95d9-748592e51c0c)
Diagram of the powerup system
![image](https://github.com/jtkardon/imgd4000-development-portfolio/assets/93606493/68d5c45b-fd4c-45a8-8bd6-83c967e85081)
Logic for choosing which powerup to give out
![image](https://github.com/jtkardon/imgd4000-development-portfolio/assets/93606493/823bfc89-cbf6-4064-ac7a-bd30caa8964c)
State Machine For Animations


Version Control:
- We used GitHub for our version control
- Since most of the tech team was already familiar with GitHub we didn't have much trouble at the start
- We set up our GitHub so that no one could commit directly to main and we needed at least two reviewers on each pull request in order to make sure that main was always functional
- We quickly learned about the fact that only one person can edit each blueprint at a time
  - There were a few instances were there were merge conflicts since people modified the same blueprints, so some people had to redo their work
  - Our orignial solution to this problem was to just ask on our discord server if anyone was using a blueprint that we wanted to use
  - Eventually, we created a specialized channel in our discord where we say which blueprints we are currently working on to make everyone aware
- Since most of the art team was not familiar with the intricities of GitHub, we had to teach them how to properly use it
- One way we could improve this in the future would be to have a trello board that lists all of our names and each blueprint, and we assign each blueprint to ourselves so we will with 100% centainty know which blueprint everyone is using.

Lessons Learned:
- Unreal is a very powerup game engine but because of that, many features are complicated. Make sure to take the time to learn all about the system you are working on to make it the best it can be
- Attempt to get the animations not at the last minute so you can see how your entire game looks
- Always pull from main when you are working to prevent any merge issues
- Utilize the plethora of tutorials on Unreal to quickly get an understanding of its mechanics so you can push them as far as you need
