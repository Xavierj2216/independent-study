# Blog IV: Back to Unity

This week I was mainly focused on Unity because I finish the EarSketch song that I needed to create for the game. That was one of the main purposes I learned EarSketch. However, I might still go back and play around with it next time. The game is almost done, we needed a UI and menu with buttons. That was the part I tried to make this week. I started with multiple tutorials like how to create a UI, play button, pause and resume, and etc. We wanted a simple button and UI because the SEP expo is coming up soon. I started to create the button while following the tutorial, the first creation had different functions like volume with a slider, checkbox, and 3 other buttons. My group didn't want that so I had to delete it and just make two buttons, which are resume and quit. The play button is in a different scene along with the title. After creating the resume and quit buttons my group didn't like it because it looks too simple. Then I went to search again for a better-looking resume and quit button tutorial. I followed the tutorial and made two buttons with C Sharp code, but the code didn't work so I had to delete it. That was all for the resume and quit buttons. Now I need to make the play button. I found a tutorial for that and made it in school. I saved the file but realize I send myself the wrong file when I got home. Finally, I recreated the play button and added a title and send it all to my groupmates. 

#### UI and buttons 

#### First video I looked at
  + How to make UI in UNITY - EASY TUTORIAL: https://www.youtube.com/watch?v=_RIsfVOqTaE
  + We wanted a simple UI, so I didn't do much after watching this tutorial

#### Second video I looked at
  + UI Introduction - Simple Menu - Unity 4.6 Tutorial: https://www.youtube.com/watch?v=rsZM3q74Q2k
![UI](https://i.ytimg.com/vi/rsZM3q74Q2k/maxresdefault.jpg)

+ What I created from the tutorial

![First](Annotation.png)
+ Then I simplified it to only the PLAY GAME button
+ I put that in one scene and two copies of that button in another scene 
+ Rename the two buttons to Resume and quit

#### Third video I looked at
  + After sending the buttons I create from the second video, it was too simple and so I had to look for a better-looking button.
  + PAUSE MENU in Unity: https://www.youtube.com/watch?v=JivuXdrIHK0
+ What I created from the tutorial

![Pause](PAUSE.png)
+ I copied this button and dragged it down to create a quit button
+ I added the C# code, but there were a lot of errors so I decided to delete it
```C#
using System;
 using UnityEngine;
 
 public class pause : MonoBehaviour
 {
     bool paused = false;
 
     void Update()
     {
         if(Input.GetButtonDown("pauseButton"))
             paused = togglePause();
     }
     
     void OnGUI()
     {
         if(paused)
         {
             GUILayout.Label("Game is paused!");
             if(GUILayout.Button("Click me to unpause"))
                 paused = togglePause();
         }
     }
     
     bool togglePause()
     {
         if(Time.timeScale == 0f)
         {
             Time.timeScale = 1f;
             return(false);
         }
         else
         {
             Time.timeScale = 0f;
             return(true);    
         }
     }
 }
```
#### Fourth video I looked at
+ START MENU in Unity: https://www.youtube.com/watch?v=zc8ac_qUXQY
+ I basically created the PLAY button shown in the video and changed the color to gray.
+ I also used the same font and color to create a UI title.
![Fourth](https://i.ytimg.com/vi/zc8ac_qUXQY/maxresdefault.jpg)


# Takeaways
1. **Communicate with your groupmates (clearly):** The reason why I had to continuously change the button and the visual appearance was because we didn't have clear communication of what we want. In the beginning, I was just told to make UI and buttons. 
2. **Tutorials provide great help:** I learn faster with tutorials compare to just diving right into the program and try to figure things out.


