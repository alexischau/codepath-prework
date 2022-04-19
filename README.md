# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Alexis Chau

Time spent: 2 hours

Link to project: https://sugary-hot-check.glitch.me/

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] Have an unlimited amount of steps in sequence (can never win, just lose)
- [x] Keep track of how many clues player got correct

## Video Walkthrough (GIF)

![](https://i.imgur.com/stcD15V.gif)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
- https://www.wikihow.com/Code-an-Alert-with-a-Variable-Using-Javascript#:~:text=Type%20%22alert%20(%22Hey%2C,%22Heya%2C%20Trevor!%22.
- https://www.joshwcomeau.com/snippets/javascript/random/

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

A challenge I encountered in creating this submission was trying to get different numbers to be in in list of sequence every time (get a new sequence every time). I looked up how to randomly choose a number between a range and had used the method (Math.random) that most sources were suggesting, but when I ran it, sometimes the sequence would stop playing. I knew it had to be an issues with the numbers being generated because when I manually put in numbers, it worked fine. After a bit more research, I believe the reason that I was having that issue was because 0 was included in the possible numbers that could be generated, which has no button associated with it. I changed add 1 to the generated number to account for this and it finally worked. Another challenge I ran into while creating this game was after making two new buttons and adding their respective numbers to the pattern list, I wasn't able to get it to play any sound when I clicked the button. I started messing around with various functions trying to get to the root of the problem and see where I needed to modify something in order to make the button work correctly. Since I was blindly changing things earlier and didn't find anything, I decided to look a lot closer into the functions and truly understand what each line was doing to find the specfic function that was connected to the sound beign played on press. I finally found a line where freqMap was being indexed into and saw that every other button had a frequency number connected to it except the new ones, so I after adding the new frequencies, a tone played after all button were pressed.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

One question I had while working on this project was what other attributes could I customize that weren't written in the writeup. I am quite unfamiliar with web development but I am sure that size, shape, and color aren't the only attributes that one can customize and would like to know more about different ways I can modify the appearance/function of the buttons that I haven't thought of and how that extends to the development of websites I've seen. I would also like to learn about different parts of a website that aren't buttons, title, or paragraphs. Another question I had while working was how to know when you should stop adding features to your website and leave it be or should there always be things added to/changed about a website. While thinking of more features I could add to the game, I started off stumped, as I didn't think there was anything else I could add to make the game better. After thinking for a bit, I could only think of two more ways I could add to the game. As someone who uses websites/apps daily, I feel as though they are always updating and changing aspects, so I am just a bit curious on how one can continually update a website with new and improved features.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

If I had a few more hours to work on this project, I would spend time trying to figure out how to pick up the playback speed every turn. I tried multiple different ways to change the delay speed but every time I made an adjustment, the pattern would not play at all. I thought I knew what each part of the function was doing and changed the right part, but I think there may have been a nuance I wasn't taking into consideration that messed up the entire function when I changed one thing. I believe if I had more time to spend on truly understanding what everything in that function was doing, I could figure out where to adjust in order to get the final result I want. Aside from the increased playback speed, I would have wanted to add images on top of the buttons. I tried to look up how to add pictures to buttton but when I tried, I think the picture wasn't in the correct size so it just showed a default picture icon. If I had more time, I would have used it to determine the real reason for the default icon and if it actually was the size, learn how to adjust the size of a picture within the scripts. Lastly, I would also have liked to research the frequency of the sounds a bit more in order to create notes that could play a recognizable song.



## Interview Recording URL Link

[My 5-minute Interview Recording](https://www.dropbox.com/s/le9ii4c8ybpmi81/video1131275218.mp4?dl=0)


## License

    Copyright Alexis Chau

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
