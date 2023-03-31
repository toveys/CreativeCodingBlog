---
title: Third Post
publish_date: 2023-03-31
disable_html_sanitization: true
---

# Final Design

For my final design I changed all the code with weird classes into code that was formatted the way we learned about in class.
I also tweaked alot of the speed values, and some of the random variables since the code I took inspiration from was designed for the full screen and mine was designed for a much smaller canvas. I tweaked the code so that the columns of symbols would drift down the canvas slower and also added less randomness in the speed. I found that large variations in speed would be too distracting. I also had to shorten the column lengths so that they didn't overlap when they looped back around when they hit the bottom of the screen. 

My biggest code changes were in the random char generation method. I added the ability for it to cycle through Katakana unicode, numerical values, as well as the Latin alphabet. This created more variation in the animation which I think makes it more interesting and engaging for the viewer. I didn't need to make my code look exactly like the matrix title, I just wanted it to be reminiscent of it. 

I also changed the opacity of the generated symbols so that they would appear to be in the background while my RMIT text could sit in the foreground and be comfortably readable. I changed the font color to a green to better match the theme of what I was going for. I also tried to have the RMIT text glow but I couldn't get it to work. I also tried have multiple copies behind it like a low opacity shadow but in the end I decided that it was more distracting than it was beneficial. I also decided to choose a font that was monospaced to have a more coding type vibe, with the monospaced font also spreading the letters out onto the screen. I really enjoyed the look of my final design, it looks sleek and I enjoy watching the numbers change as they go down the screen.

If I were to do this project again I would add some more randomness to it. I noticed that the column lengths once generated in the setup, don't change at all in the draw function. The column lengths and speed remains the same, just the text itself changes. If I were to repeat this, I would make it so that the columns would vary in size and speed every time they hit the bottom of the screen. I would also want to figure out how to make the middle text glow and have a streak effect to the sides so that it realy pops against the background. While it is nice currently, it feels very static so I would have it change subtly.
<iframe src="https://editor.p5js.org/toveys/full/Ut74ha7vb" width="576" height="366"></iframe>