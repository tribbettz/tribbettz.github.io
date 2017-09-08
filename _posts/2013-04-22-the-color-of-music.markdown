---
layout: post
title: "The Color of Music"
date: 2013-04-22 16:48
published: true
categories: [Expression, Perspective, Electronics, Media Lab, Open Source]
---

Can your voice be represented with a color? What would a drawing look like of an entire dance sequence? Can you taste sound? 

I was thinking about these questions for a class I'm taking called <a href='http://web.mit.edu/4.110j/www/' target='_BLANK'>Design Across Scales</a>. It's a phenomenal class, taught by Professors Neri Oxman and Meejin Yoon in the MIT Media Lab. 

The most recent project for the class was to _Make Something that Makes Something_. I thought okay: I make expressions. I make art. I make music. So I can make a new _technique_ that uses many senses at the same time to make something - a drawing, a color, a taste. I'm calling it _Multi-Sensory Expression_. 

<!-- more -->

![My image]({{ site.url}}/images/color_of_music.jpg)

I'm definitely not the first person to think about expressing myself using multiple senses. YOU do it, too! Everyday, you deliberately put on matching clothes (vision), you spray yourself with perfume (olfaction, smell), and you hopefully brush your teeth for your significant other if you're dating (taste)*. So there you go! Even before you leave your house in the morning you've expressed yourself using __three__ different senses. Bravo! Well done to you!

During my brainstorming process, I came upon a project called <a href='http://web.media.mit.edu/~silver/drawdio/' target='_BLANK'>_Drawdio_</a>, which was developed by Jay Silver in the MIT Media Lab. It's a  "pencil that lets you draw music" using a <a href='http://en.wikipedia.org/wiki/Theremin' target='_BLANK'>Theremin</a> (an electronic musical instrument). It inspired me to think of a whole bunch of awesome tools I could build to express myself in brand new ways. But for the class, I decided it would be cool to generate a colorful picture from listening to music and _watching_ me dance. 

![My image]({{ site.url}}/images/arduino_motion_sensor.jpg) 

I did this by developing two modules. The first module changes the color of a circle based on the _loudness_ of the music or sound. The second module changes the position of the circle based on _location_. I used the <a href='http://www.processing.org/' target='_BLANK'>Processing Language</a> to build my app which listened to music input over the microphone and read arduino serial input from an ultrasonic motion sensor. My program took both these inputs and translated them into _circle colors_ and _circle locations_. 

The idea is that now you can dance to music in your room with this circuit sensing your position and creating a picture of those awesome moves you just showed off. It's a new way to represent dance. It's a new way to think expressively; Multi-Sensory Expression.

I put the code on <a href='https://github.com/tribbettz/multi-sensory-expression' target='_BLANK'>my github</a>. It's a simple example and this idea has a long way to go. I'll be posting updates as I upgrade but I think that this little prototype - for as simple as it is - allows you to now express yourself in a way that your previously couldn't...that's pretty groovy.

Now go out and dance your tukas off to the sweet tunes of spring coming into bloom; Happy Earth Day!

\* My mother - a dental hygienist - highly recommends brushing your teeth three times a day, everyday; not just when you're dating.
