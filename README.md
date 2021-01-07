# cody
Personal text editor 

TODO:

* Read lines from file and parse them into workable format
  * Seperate file lines into ?elements?
  * Manager for elements to reorganaise lines, add, remove, splir
  * convert elements into lines and write to disk
* Edit mode
* Dynamic search highlighting 

* Font is fixed 8x16 pixels
* On scale below certain limit canvas and other elements scale down decreasing effective usuable space but below that resolution entire program is scaled down instead of individual elements. 

There arw two different self sustaining cores
* Dispaly system is responsible for drawing lines in current char grid it made, breaking lines on overflow, any visual cues and effects
* Text system is responsible for keeping lines in memmory, breaking lines on new line symbol or connecting lines, text system needs to be able to dynamically change maximum lenght of line to accomidatie bigger footprint.
