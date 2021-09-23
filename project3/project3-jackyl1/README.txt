Project 3: TouchOSC Control
Jacky Liu
jackyl1

To run: 
 1) In TouchOSC, set port to 8213 and ip address to the one on your pc.
 2) Make sure the layout in TouchOSC is set to Autobat5 (the first/default one)
 3) Open cmd/terminal in this directory (with init.srp)
 4) Run wxserpent64
 5) Either press the start button in the wxserpent GUI or press the 
    start button in the controls mentioned below

 Note: The cmd/terminal will print out values indicating what you're playing
       as you adjust the sliders/buttons.

 WARNING! Messing with the controls in the GUI in wxserpent for pc
          at the same time as on TouchOSC may screw up things! (Those
          controls on wxserpent exist because this is based on project 2)

Controls:
 * There is a png file attached showing a mapping of the controls called controls.png *
 * Below are also more detailed instructions on controls *

1) Bottom Gray Slider: Tempo
 - 0.05 - 1.05 BPS (beats per second)
 - This slider is called "/faderM" in the code.

2) Left Green Button: Start
 - Starts playing sounds
 - Will not play duplicates if you press twice (limited to 1)
 - The button has a shade in animation, but it does nothing. Please ignore it. 
   Pressing the button once regardless of its state will start playing sounds.
 - This button is called "/toggleA_1" in the code. 

3) Left Red Button: Stop
 - Stops playing sound
 - This button is called "/toggleB_1" in the code. 

4) Green Slider: Volume (velocity) for Sound 1
 - 0 to 127 velocity units (bottom is 0, top is 127)
 - This slider is called "/1/faderA" in the code. 

5) Red Slider: Volume (velocity) for Sound 2
 - 0 to 127 velocity units (bottom is 0, top is 127)
 - This slider is called "/1/faderB" in the code. 

6) Blue Slider: Chord Note for Sound 1
 - Changes the note for the chord anywhere from C to B (C is bottom, B is top)
   letting you pick C, C#, D, D#, E, F, F#, G, G#, A, or B.
 - This slider is called "/1/faderC" in the code. 

7) Yellow Slider: Chord Note for Sound 2
 - Changes the note for the chord anywhere from C to B (C is bottom, B is top)
   letting you pick C, C#, D, D#, E, F, F#, G, G#, A, or B.
 - This slider is called "/1/faderD" in the code. 

8) Blue Rotary: Octave for Sound 1
 - Changes octave between 2 and 6. 
   For example, 4 means it plays notes in the 4th octave, such as
   C4, and F#4. 
 - This rotary is called "/rotaryC" in the code. 

9) Yellow Rotary: Octave for Sound 2
 - Changes octave between 2 and 6. 
   For example, 4 means it plays notes in the 4th octave, such as
   C4, and F#4. 
 - This rotary is called "/rotaryD" in the code. 

10) Left blue button: Toggles major scale for Sound 1.
    Code is "/toggleC_1"
11) Right blue button: Toggles major 7th scale for Sound 1.
    Code is "/toggleC_2"
12) Left yellow button: Toggles minor scale for Sound 1.
    Code is "/toggleD_1"
13) Right blue button: Toggles dominant scale for Sound 1.
    Code is "/toggleD_1"



