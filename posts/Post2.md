---
title: Second Post
publish_date: 2023-03-25
disable_html_sanitization: true
---

# Prototype 2

After a couple of days watching Coding Train videos, I found a great Coding train video where a guest named Emily Xie walked through the steps of creating their own Matrix inspired animation. 
<iframe width="853" height="480" src="https://www.youtube.com/embed/S1TQCi9axzg" title="Guest Tutorial #4: Matrix Digital Rain in p5.js with Emily Xie" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
They also included another variation of their code on Github, which was their final piece that they tidied up. This version wasn't as legible as the
one from the video but I did see some things in there that I thought could help me on my assignment. 
<br></br>

![green rain inspo](../images/green_rain.gif)
[Inspiration from another P5 Sketch](https://github.com/emilyxxie/green_rain)

I based my second prototype pretty heavily on what they taught in their tutorial, but interestingly enought they had a small error in theor code which I fixed in mine. After staring at my screen for a long time, I noticed that there was a weird looking unicode char that popped on screen for a couple of milliseconds. It was barely noticible but I decided to fix the mistake so that I could have something of my own in the code. I realized that when they generated a random katakana char between two unicode values, they actually went one value too far, and hit an undefined unicode value. 

 `0x30A0 + floor(random(0, 97))`

 I fixed this problem in my code, it was a very small error but I felt good that I was able to tweak their code and understand it. In their final piece I saw that they their symbols cycled through Katakana as well as numbers, which I really liked so I added that to my sketch as well. They also must have been using an old version of p5, because the way they defined their classes was different to how classes were discussed during our class.
 They seemed to be defining it like a function with arguments, there wasn't a constructor, and their methods were written kind of weird.

```json
function Symbol(x, y, speed, first, opacity) {
  this.x = x;
  this.y = y;
  this.value;

  this.speed = speed;
  this.first = first;
  this.opacity = opacity;

  this.switchInterval = round(random(2, 25));

  this.setToRandomSymbol = function() {
    var charType = round(random(0, 5));
    if (frameCount % this.switchInterval == 0) {
      if (charType > 1) {
        // set it to Katakana
        this.value = String.fromCharCode(
          0x30A0 + floor(random(0, 97))
        );
      } else {
        // set it to numeric
        this.value = floor(random(0,10));
      }
    }
  }
}
```
They were classes but since they weren't written like the classes we learned I decided that I would rewrite the code in my final sketch so that it would have new ideas in it as well as be in the formatting that we were taught.
<iframe src="https://editor.p5js.org/toveys/full/a9b-xY2GF" width="576" height="366"></iframe>
I also met up with a classmate outside of class since they were also having trouble with classes. We went over each other's projects and gave each other a critique of what we had design wise. Since they didn't understand classes very well and I kind of did, I took a shot at explaining it as well as looking at their code and giving them ideas on where to use classes. They had multiple texts in their canvas, each with a different font style, font color, and font size, so I helped them create a class that had a constructor and fields for these values as well as a method that could be called to draw the text on the canvas. This was pretty simple, but trying to explain what a class is and what it does to someone else definitely helped me understand it a bit more, and I hope they understood it more as well.