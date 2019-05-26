# Blog IV: Final touches to project

This week our group finish the MVP and we are going to add some final touches for presentation. The texture of the mountain needs some improvement and we want to add things like loading menu, and a new song for the main menu. We do not know if it will be completed before the presentation, but we are working on it. I am in charge of adding those two features to our game. I looked at lots of tutorial and went back to EarSketch to create another song. The difficult part was with the loading menu. Even though, it was easy to create one just with Unity it does not look good. The visual looks too simple and plain. The song was made during this week, but my group does not think it flows with the other music that is already in the game. I also created a loading screen by using free to reuse images. 

### Loading menu

#### Simple loading menu
  + Unity 5: Loading Screen/Bar: https://www.youtube.com/watch?v=rXnZE8MwK-E
  + This was one of the video I watched, the loading menu below looks a little plain 
  + The font and the color looks simple too, with a gray background
![simple](https://i.ytimg.com/vi/rXnZE8MwK-E/maxresdefault.jpg)
  + This is another simple loading screen I watched
  + How to make a LOADING BAR in Unity: https://www.youtube.com/watch?v=YMj2qPq9CP8

#### Complex loading menu
  + Unity Loading Screen Tutorial | How To Create A Loading Bar In Unity: https://www.youtube.com/watch?v=u1Fwm5eGYrc
  + The video was pretty long showing all the steps taken to make a loading menu 
  + The problem with this tutorial is he used a image
  + I have to be able to use that image or else I can not create the loading menu
  + This is when I realize I should get free to use images for my loading screen
![complex](https://i.ytimg.com/vi/u1Fwm5eGYrc/maxresdefault.jpg)

#### The video that helped most
  + How to make a LOADING screen in Unity!: https://www.youtube.com/watch?v=fxxoACKCWVo
  + I did not create the loading menu shown in the video because that requires an asset
  + Last time I had trouble exporting an asset to my group
  + It also takes up a lot of space making the game hard to run and lag.
+ What I created after watching the video
  + I used two images one for the background and the other for the slider or loading bar
  + ![back](https://www.publicdomainpictures.net/pictures/230000/nahled/future-downloading.jpg)
  + ![bar](https://upload.wikimedia.org/wikipedia/commons/e/ed/Progressbar100.png)
+ I used both images and combine them to create a loading menu
+ I rescale the size and change the color to fit our game

### EarSketch
+ This is the new song I created, the code is shown below
+ It is also calm, but it does not flow with the other song in the game
+ Still working on it
```python
#		python code
#		script_name:
#
#		author: Xavier
#		description:
#

from earsketch import *

init()
setTempo(120)

fitMedia(Y11_PIANO_1,1,1,21)
fitMedia(Y33_PIANO_1,2,5,13)
fitMedia(Y33_PIANO_2,3,5,13)
fitMedia(Y41_PIANO_1,4,10,15)
fitMedia(Y54_PIANO_1,5,15,20)
fitMedia(FOXTRICK_RAIN_WATER_DRIPPING_SOFTLY,6,1,10)

setEffect(2, VOLUME, GAIN, -20)
setEffect(3, VOLUME, GAIN, -12)
setEffect(4, VOLUME, GAIN, -12)
setEffect(6, VOLUME, GAIN, 5)
finish()

```
### Next step
+ To get ready for presentation
+ Prepare slides and fix bugs or visual features of the game

# Takeaways
1. **It doesn't have to be exactly the same:** Tutorials are there for us to learn, sometimes we can follow step by step. However, other times we can use what we learn to create something new.




