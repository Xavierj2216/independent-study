# Blog III: EarSketch tutorial and music

Now I have learned a lot of the basics in EarSketch and understand how to make a song. During this week I was looking at more 
functions in EarSketch and creating different music. I have multiple files with complete songs, but these songs aren't good. That is why I need to work more on the transition between different clips and to create a more catchy beat. I also saw many videos and guides on how to write lyrics, create good melody, make beats like some popular DJs, and etc.  

### Learning EarSketch
The music or code I was working on in EarSketch python script. The below is only a part of it:
    
    author: Xavier Jiang
    description: Music 2
    from earsketch import *
    init()
    setTempo(120)
    # Music
    # drums1 = RD_ROCK_POPRHYTHM_DRUM_PART_10
    beatFill = RD_ROCK_POPRHYTHM_MAINDRUMS_1
    drumFill = RD_EDM_DRUMBEATPART_1
    # Clip
    insertMedia(RD_POP_SFX_FMDOWN_1,1,1,3)
    fitMedia(RD_POP_PADCHORD_2,2,2.9,6.9)

#### The basics, the keywords and functions in EarSketch

+ str() - convert any value into a string.
+ int() - convert a string containing digits into an int.
+ float() - convert a string containing digits with a decimal point into a float.
+ Set and make variable
+ Different signs/symbols and their use (+,=,*,\,-)
+ Expression: any code that returns a value.

Most of the tutorial shows python code being convert into Earsketch code. Then a comparison between the two codes like how to use each.
Ex: Variable in EarSketch
tempo = 120
or
clip = "YG_HOUSE_PERC_1"

+ The insertMedia() function is what allows you to place sound clips into the EarSketch DAW. The function takes in 3 parameters:
    + clipName
    + Track- the location of the clip in the DAW
    + startMeasure: where to place the clip on the track

+ setEffect(). It allows you to apply audio effects to your tracks to enhance the sound. This function takes in 4 parameters:
    + track: An int specifying the track to add the effect to.
    + effectName: A string (constant) specifying name of the effect (e.g. VOLUME)
    + effectParam: A string (constant) specifying the parameter of the effect to set (e.g. GAIN)
    + paramValue: A float specifying the value of the effect parameter.
    
+ Effects with setEffect method
    + VOLUME (how loud a track is)
        +Method: GAIN
    + PAN (best heard with headphones, this is where the sound lies from left to right)
        +Method: LEFT_RIGHT
        +Ranges from -100.0 (all the way left) to 100.0 (all the way right) with 0.0 being in the center.
    + DELAY (adds echos to the sound)
        +Method: DELAY_TIME, MIX
        +Ranges from 0.0 (no delay) to 4000 (4 second delay).
    + DISTORTION (makes a sound lofi and noisier)
        +Method: DISTO_GAIN
        +Ranges from 0.0 (no distortion) to 50.0 (maximum distortion).

+ My EarSketch (This is a overview, the detail inside is not important)

    <img src= earsketch-progress.png />
    

### Learning Music
 
+ One of the music producing video I watch: 
https://www.youtube.com/watch?v=OEIk3bJtTNw
   <img src= "https://i.ytimg.com/vi/OEIk3bJtTNw/maxresdefault.jpg" />

The other videos I watch were either EarSketch or song breakdown like Faded by Alan Walker.
I also did a lot of exploring with catchy beats, good edm music, famous artist producing, writing lyrics, writing rap, etc.
As I learn I did revision to my own music and ask suggestions from family, friends, and classmate.

   + One example for writing lyric: http://blog.sonicbids.com/how-to-write-lyrics-for-the-first-time
   + Most good melodies use repeating elements.
   + Rhythm & Varying Note Lengths
   + Combine notes that are next to each other

# Takeaways
1. **Always remember to learn the basic, but don’t just learn do it:** I read and looked at a bunch of tutorials but I forgot half of it because I never tried it out myself. In the past I heard others say to use the code while you learn now I know why.
2. **It is easy to create something but hard to make it good:** I created multiple beats/song but it is really hard to make it catchy or have great melody.
3. **Ask for suggestions** Throughout the process of making music I ask multiple people what they they about the song and what I should add. This is for improvement in my music. 
