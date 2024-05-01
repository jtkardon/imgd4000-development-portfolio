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
- Numerous bug fixes and quality of life changes

Challenges:
- One of the first major challenges I faced was learning Unreal and blueprints as I had never used them before. It took some time for me to start understanding how blueprints work and what the important nodes were. I overcame this challenge by watching many tutorials on the inner workings of Unreal and the basics of blueprints.
- A major challenge that we faced was fixing an issue with the animations where it would freeze if you pressed the key in rapid succession. We got everyone on the team together and put our heads together in order to try and find a fix. After much trial and error, we fixed it by setting the animations to loop and modifying the way the key presses were setting the variables.
- Another challenge I faced was when I didn't pull fully from main after creating a branch in order the make the credits page, so there were merge conflicts with the menu blueprint and I thought that I would have to redo the entire credits page. I got around this by copying all the widgets of the credits page to another ui blueprint that was not being touched, pulling from main and then copying it back into the main menu blueprint. This saved the few hours of work it would've take me to redo the page.
  
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
