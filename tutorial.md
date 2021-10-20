---
moduleid: 0
title: Template as template
published: True
slug: template-template-template
---
# Sequence: Ambient Computing: Interactivity
## Sequence Summary:
This sequence of modules introduces concepts of interactivity in ambient computing as well as Processing. 
## Why?
Processing is a flexible software sketchbook and a language for learning how to code within the context of the visual arts. Its an especially great environment for ambient computing because it will allow you to prototype projection mapping that responds to interactive inputs like (a web cam, markers, or a multitude of triggers from the web). Many artists choose to work with Processing because of its visual interface and its simplicity.
## Modules:
Intro to Processing - Lighting
Webhooks
Sounds, Speech and Macros
Markers and Tracking
Computer Vision

Template for Modules:
===========================================

# Grasshopper as Tool-making Medium: Levels of Abstraction: Clusters and Plugins
## Module Summary

labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Conceptual Introduction, or: Why is this interesting / important?

labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
## Tutorial

![blahblah](0-template-gif.gif#img-full)

1. **Download Processing.**  
Place [Processing](https://processing.org/download) in the Applications folder on your computer (or Program Files for Windows). When you double click Processing, it should install and launch the application with a new empty sketch. A sketch is where you will write your code. We’ll be writing code in Java inside of Processing.

2. **Basics**  
Processing includes 
   * a text editor - where you write your code (called a "sketch" in Processing)
   * a compiler - translates code written in a high-level language into a set of machine-language instructions that can be understood by a digital computer's CPU 
   * a display window - where visuals created by your sketch are displayed

VIOLET INSERT DIAGRAM (IDE :toolbar play/stop, text editor, console/errors, sketch)

You will have two basic parts within a Processing "sketch", the **“setup”** and the **“draw”** loop. The setup loop runs once when launching your script, whereas the draw loop runs repeatedly. This allows you to save computing power by sticking parts of the code that only need to run at the start in the setup loop. The draw loop will continually update so it can change over time, or get realtime information such as the location of your mouse or update a camera feed.

```
void setup() {
  size(1280, 960);
}
  
void draw() {
  background(0);
  ellipse(mouseX,mouseY,500,510);
}
```

VIOLET EXAMPLE INSERT HERE - draw and setup in action

3. **Documentation Intro**  
The basis of learning to code is really about learning how to find and use information (usually online). Rarely does anyone know off hand the exact syntax and operations to write all of their code from scratch. Rather, creative technologists and even seasoned software engineers regularly use the documentation pages for a programming language or a development environment to understand how a particular programming language functions, its operations, and so they can borrow from what's already written.
You can find Processing's documentation here:
[Processing Documentation](https://processing.org/reference/)

4. **Using Documentation**  
If we look around within Processing's documentation, we'll see all kinds of operations and parameters we can use in our code. So much possibility! Poke around and click into some of the functions you see. Lets look into `background()`. You'll see if we click into [background](https://processing.org/reference/background_.html) we'll get information on how to use this function, what parameters it expects, and some examples. It looks like it takes a single number `background(51);` for a value between black and white, or 3 numbers `(background(152,190,100);` for RGB values.

**CHALLENGE**  
Can you change the background to yellow?

Here are some other fun functions to play with in your sketch.
```
fill()
noFill()
stroke()
brightness()
color()
hue()
saturation()
```

**CHALLENGE**  
Can you change the fill and stroke of the ellipse?

5. **Understanding the Draw Loop**  
Remember the draw loop runs continuously so you can build interactive functionality. Lets take advantage of this to see other ways we can get our ellipse on the screen to move. You can think about your sketch as one big long formula


![alt-text](images_can_be_named_anything.png#img-left)

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

![more alt-text about image](images/images_work_in_subfolders.png#img-right)



Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

<div class=”video”>
<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/603252807?h=28246f992b&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Introduction to Rhino 1 of 3: Interface"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
</div>

Code block:
```
console.log("hello world");
console.log("hello world");
console.log("hello world");
```

The End!!
