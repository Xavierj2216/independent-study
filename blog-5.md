# Blog IV: EarSketch collaborate project

I am done with my EarSketch learning and from now on I will be more focus on the music. I am planning to make music for a group project
that will be on Unity. It will be the combination of Unity, EarSketch, and Blender. This week most of the music and beats I play around with are for the game. The music should be calm, the past music I produce are mostly upbeat or pop. I was using a lot of sounds from Freesound because EarSketch doesn't have much sound effects I want. I will listen to different instruments, beats, and then download it into EarSketch. Then I would combine the beats that sound good together. Most of this week is tinkering, deleting parts, and replacing. I will still go back and review the EarSketch functions and maybe search for the parts I need. 

#### The keywords and functions in EarSketch
+ Data structures store a collection of values in a single entity. 
+ Indices are used to refer to individual elements of the structure. 
+ A for-loop provides a simple way to iterate through an entire structure
+ Nested loops are loops within a loop, that can be used to sort through multi-dimensional data.
+ A stopping condition is what causes a function to stop running.

+ Lists 
  + are a good way to store data used for Sonfication.
  + A multi-dimensional list combines multiple lists
  + A list is a way to store and index variables.
  + A list can be reordered.
  + Lists are useful for storing and sorting properties of sound.
  
+ Sonification 
  + is a way to use audio to convey information, by turning data into sound. 
  + Sonification has a lot of useful applications, like helping the visually impaired through sound. 

+ + rgbToHex() which changes three numbers to its hex value.

+ The analyze() function 
  + allows you to find the volume of the sound with RMS_AMPLITUDE. 
  + analyze() also lets you work out how bright or dark a sound is with SPECTRAL_CENTROID. 
  + Ex:
```python
clip = YG_TECHNO_ELECTRIC_PIANO_2
analysisValue = analyze(clip, RMS_AMPLITUDE)
print analysisValue
```

+  importImage function 
  + that converts any image into data that can be used within EarSketch
  + importImage(imageURL, numberOfRows, numberOfColumns)
  + It’s usually easiest to use a black and white image.
  + Ex: 
```python
myImage = importImage("http://earsketch.gatech.edu/wp-content/uploads/2013/03/grid_zoomed.png", 8, 8)
print myImage
```

+ onLoop() must be used for all scripts in EarSketch that create visualizations.
```python
def onLoop():
  drawRectangle(10,15,50,30,"#FF0000")
```

### One music for my calm sound
```python
from earsketch import *

init()
setTempo(120)

fitMedia(FOXTRICK_PIANO,1,1,30)
setEffect(1,VOLUME,GAIN,-1)
fitMedia(FOXTRICK_OCEAN_NOISE___SURF,2,5,24)
fitMedia(FOXTRICK_GUZHENG,3,6,20)
setEffect(3,VOLUME,GAIN,-2)


finish()

```

### FreeSound

![free-sound](https://upload.wikimedia.org/wikipedia/commons/3/3c/Freesound_project_website_logo.png)

![free-sound](https://d2.alternativeto.net/dist/s/2fc76370-86f9-e011-98e6-0025902c7e73_1_full.png?format=jpg&width=1600&height=1600&mode=min&upscale=false)

### Game plan
+ Like a walk in a park
+ Probably 3D, look at the nature or landscapes
+ Human looking model for character
+ Able to move around
+ Music playing in background


# Takeaways
1. **Be willing to change your style for the team:** I like music that are more hype or upbeat, but the game is more calm so my music should fit that category.
2. **Use all the resources that can help you and don't limit your own ability:** I won't limit myself because EarSketch doesn't have a lot of sound effects, I would search online for resources like FreeSound. Create a project you like, so you won't have any regrets.

