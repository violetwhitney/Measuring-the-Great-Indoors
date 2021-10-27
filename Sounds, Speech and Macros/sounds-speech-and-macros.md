temp

Playing Sounds
From Processing go to Sketch → Import Library→ Add Library → search for “sound” and select “Sound | Provides a simple way to work with audio” → and click ↓ Install.

2. Now in your Processing sketch copy in the following code from the codeblock below. You can also download the sketch from here.
Do not press play just yet! You need to first add your sound file (.wav file or .aifff) to your Processing sketch folder.
import processing.sound.*;
SoundFile file;
void setup(){
  size(800,800);
  background(255);
  
  //this loads the file based on the file name
  file = new SoundFile(this,"stampede.aiff");
  file.play();
  
  //this changes the volume level (number between 0 and 1)
  file.amp(.5);
}
void draw(){
}
3. You can download stampede.aiff here or download goat.wav here. These are the sound files we would like Processing to play.
4. Save your Processing sketch. The name of your Processing folder must match the name of your Processing sketch as shown in the image below.
Drag and drop the sound files you’ve just downloaded into your sketch folder as shown in the image below. Now when you press play from Processing your sound file should play.

5. You can find more free sounds by creating an account at https://freesound.org/ and downloading your own files that you would like to play.


Listening to Your Mic
To listen to the mic on your computer copy and paste the text from below. You can also download this Processing file directly from here.
import processing.sound.*;
AudioIn input;
Amplitude analyzer;
void setup() {
  size(200, 200);
// Start listening to the microphone
  // Create an Audio input and grab the 1st channel
  input = new AudioIn(this, 0);
// start the Audio Input
  input.start();
// create a new Amplitude analyzer
  analyzer = new Amplitude(this);
// Patch the input to an volume analyzer
  analyzer.input(input);
}
void draw() {
  background(255);
// Get the overall volume (between 0 and 1.0)
  float vol = analyzer.analyze();
  fill(127);
  stroke(0);
// Draw an ellipse with size based on volume
  ellipse(width/2, height/2, 10+vol*200, 10+vol*200);
}

Text to Speech
Getting A Mac Laptop to Speak
Processing can execute commands outside of Processing. On macs we can make our computers do speech to text:
void setup(){
  exec("say", "hello");
}
You can also use one of your Mac’s these unique voices:
Alex, Alice, Alva, Amelie, Anna, Carmit, Damayanti, Daniel, Diego, Ellen, Fiona, Fred, Ioana, Joana, Jorge, Juan, Kanya, Karen, Kyoko, Laura, Lekha, Luca, Luciana,Maged, Mariska, Mei-Jia, Melina, Milena, Moira, Monica, Nora, Paulina, Samantha, Sara, Satu, Sin-ji, Tessa, Thomas, Ting-Ting, Veena, Victoria, Xander, Yelda, Yuna, Yuri, Zosia, Zuzana
void setup(){
  exec("say", "-v", "Karen", "hello");
}

Speaking to the Amazon Echo
You can also make your Mac speak to an Amazon Echo:
void setup(){
  exec("say", "Alexa, what time is it");
}
Or ask your echo to execute other services:
void setup(){
  exec("say", "Alexa, turn off the lights");
}
Check here for a list of arguments you can use with the Amazon Echo.


Text & Speech
Finally if you want to think more about creating custom phrases you may want to understand more about what are called strings. Strings are a data type used in programming, such as an integer 6 a float 6.2, but is used to represent text rather than numbers, i.e. This is a string but 6 can also be a string. To learn more about strings and text in Processing check out this video tutorial:

Making Bots
JSON format is particularly useful for auto-sentence generation because its dictionary format links words with keys which we can use as categories. The Corpora project is a great spot to find word lists already formatted as JSON.

As cynical start-up idea generator, Darius Kazemi
As poetry maker, Allison Parrish
Gender, Kate Compton
Magic Realism, Kate Compton

Projects that Use Sound




Could you add a rainforest sound to a room everytime a person walks in the door, until you have a complex rainforest?

Could you play with the idea of who is speaking in a room, and direct light towards them?
https://vimeo.com/groups/processing/videos/3102434
