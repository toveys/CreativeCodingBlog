---
title: Ninth Post
publish_date: 2023-05-29
disable_html_sanitization: true
---

# Final Design

While working on my final design I worked out as many of the bugs with the recursive functions and the audio issues as I could.
I was unfortunantly not able to have the canvas "fade out" after a song ended which I thought would be easier on the eyes, I just couldn't get the timing quite correct since the recursive function I was using was running a lot faster than I wanted it to. I wanted to apply a somewhat transparent black background onto the canvas every frame for around a 2 second fadeout time but the fadeout would happen instantaneously. I decided to give up on this since I wanted to add in some variations to my main circular audio visualiser. Similar to the the ITunes audio visualiser, I wanted to have different animations happen when I load up different songs. So I decided to create at least two more main audio visualisers that would get decided randomly when a user loads a new mp3 file. I created one visualiser inspired by colorful parrots, where I used cut up circles to resemble feathers that form triangular patterns when a high frequency is sustained. Otherwise, it creates a cool tri-pronged swirl in the center. This audio visualiser works best with songs with sustained higher frequencies and little other frequencies. It creates a cool triangle pattern in the middle when such a song is playing, however it feels a bit static when songs with a wider range of frequencies play.

![Feather Theme](../imagesFinal/feather%20theme.jpg)

I also made a mushroom inspired visualiser since I know that my sister loves mushrooms and I wanted to create something that would be engaging for her. 
I decided to have the color of the mushrooms to be decided by their frequenc but also by how "tall" they grow. Since the mushroom height was determined by how much of the frequency they are assignened to exists in the song, when they "grow" they change color from a green "young" mushroom to a red toadstool. This visualiser ended up taking the most time to create since initially I wasn't too stoked on the design. The colors were blending in making the mushrooms hard to distinguish, and the spiral was relatively small so there wasn't too much complexity happening. But when I started experimenting on making the spiral bigger and making the colors determined by height, the mushroom design turned out to be my favorite of all the visualisers I made.

![Mushroom Theme](../imagesFinal/mushroom%20theme.jpg)

Overall, I think that my code has enough complexity to be engaging but there are some limitations in my project that leave me a bit unsatisfied. Mainly, the way to play music requires you to load up each mp3 file individually, and you need to have an mp3 file on hand to be able to use my code. I would have wanted to be able to connect my project to a folder with mp3s in them and have the next song in the folder play automatically when the current song is finished. What happens to the animations when I use the media controls can feel clunky, and if I pause and play too much, or load songs too fast, then my code starts to slow down a lot. Having to refesh the page every time I want to play a new song is annoying and if I were to let other people use it, their user experience would not be that great. Everything works fine when you load up a song and let it play all the way through, but obviously people still need a way to pause when they want or skip forward to a part of a song they want to hear.

I don't work with audio regularly so designing visuals that are supposed to complement and interact with audio introduced a lot of challenges that I never thought of. One of which was, what songs I was using to design the visuals. I had to test the visuals with a wide range of songs, with high frequencies, low frequencies, and a more median mix of the two. I realised that different songs interact in different ways which is a good thing for complexity, but also makes it hard if there is a "look" you want the visual to have. For instance my feather inspired visuliser feels stiff with songs that don't have mostly higher frequencies sustained. I started downloading more and more songs to test out my visualiser with in order to see how it would react. I couldn't design the visuals all around one or two songs or they visuals I liked might not appear in other songs.

During my coding process I did let my sister see what I was doing but I coded the mushroom visualiser in secret so I was getting some feedback on my project which was important, since the whole point of making this was to provide an experience that meshed with our shared values of music, entertainment, and fun that made our repertoire of eating meals together more engaging.

GitHub Code:
https://github.com/toveys/AudioVisualiser

Website Link:
https://toveys.github.io/AudioVisualiser/