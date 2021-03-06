# Blog IV: EarSketch collaborate project Part 2

This week I was mainly focused on the music production for our Unity game. I finish making a calm song that uses different instruments specifically a piano. Most of my sounds come from Freesound and of course EarSketch too. It was hard to create calm music because if I add on different sounds it won't flow or fit into the music. I had to use the functions in Earsketch to minimize the volume, and I also did some research on instruments to create a calm song and instruments that go well with piano. For example, cello, violin, and sometimes drum these are some of the instruments. This week I also struggle with the loops. Our Unity game requires the song to be long and in order to be more efficient I had to use a loop. The for loop in EarSketch was pretty confusing to me I spend days trying it and learning about it. After a few days I found a new type of loop that is in EarSketch. It is a while loop, the syntax and function is much easier to understand. Next week I will learn how to upload my music to Unity, and make other songs.

#### The keywords and functions in EarSketch
+ While Loop
  + The while statement, allows us to execute a code block repeatedly while a condition is True
  
+ The code below is without while loop
```python
from earsketch import *
init()
setTempo(120)

start = 1
clip = HOUSE_BREAKBEAT_001
length = dur(clip)

insertMedia(clip,1,start)
start += length
insertMedia(clip,1,start)
start += length
insertMedia(clip,1,start)
start += length
insertMedia(clip,1,start)
start += length
insertMedia(clip,1,start)
start += length
insertMedia(clip,1,start)
start += length
insertMedia(clip,1,start)
start += length
insertMedia(clip,1,start)
start += length

finish()
```
+ When there is no while loop the code will be long and inefficient
+ This is with a while loop
```python
from earsketch import *
init()
setTempo(120)


start = 1
clip = HOUSE_BREAKBEAT_001
length = dur(clip)

x = 1
while x < 9:
	insertMedia(clip,1,start)
	start += length
	x += 1

finish()
```
+ The basic syntax/code of a while 
```python
x = 1
while x < 5:
	x += 1
```
+ The while loop itself only takes up four lines of code and can be modified to repeat any number of times by simply changing the int in the condition. 
+ dur() function gets the length of the clip and redefine the start position with each repetition.
  
+ For loop
  + A for loop can iterate over a string in order to use one character at a time. 
```python
for letter in songPattern:
	if letter == "A":
		fitMedia(clipA1, 1, start, start + sectionLen)
		fitMedia(clipA2, 2, start, start + sectionLen)
	elif letter == "B":
		fitMedia(clipB1, 1, start, start + sectionLen)
		fitMedia(clipB2, 2, start, start + sectionLen)

	start += sectionLen
```
![for loop](Loop_Components_PY.png)

### My calm music
```python
for i in range(1,41):
  
  fitMedia(piano,1,1.5,41)
  setEffect(1,VOLUME,GAIN,-4)
  fitMedia(cello,3,6,20)
  fitMedia(violin,4,20,30)
  setEffect(4,VOLUME,GAIN,-30)
  setEffect(3,VOLUME,GAIN,-12)
  
fitMedia(FOXTRICK_OCEAN_NOISE___SURF,2,1,10)

```

### Game plan
+ We got the movement done
+ Character is being design
+ Test models are created
+ The landscape is almost done
+ Music playing in background needs to be uploaded.


# Takeaways
1. **Make your code efficient:** If there is a way to make your code efficient then use it, loops can help a lot when you are repeating the same code multiple times. 
2. **Don't worry there might be multiple solutions:** If the for loop doesn't work there is a while loop, I just have to search for it and learn. 

