# SmartMirrowMQTT-
a smal app to recycle your old android phone. Visulise Data via MQTT at your Phone.

this Project was created by the esp-32 contest by the elector magazin. Sorry for publishing so late, i already did a lot of changes.
Here the link the the Project Page. there is also na nice Idia How to bild with your Phone your smart mirror.
https://www.elektormagazine.com/labs/mqtt-weatherstation
this Android App is wirten at MIT app inventor (was google app inventor in former times). -> https://appinventor.mit.edu/

this App dosn´t alow MQTT-Password (jet).

insert the MQTT-Brocker IP-Adress at the main window. And press the Button connect. The Number next to it shows the actual state. 
0-dosn´t connect
1-connecting
2-conection broke
Black (no Numbers, IP Window or stuff)-conected

there is also an App Inventor .aia file to make changes or see inside.

_____________________________________________________________________________________________________________________________________

To visual lise your Data, just connect to the Broker and send the Data via following Topics (Node Red is a nice tool for that ;) ):
"/home/smalmirror/topic"      - the Topic/headline
"/home/smalmirror/value/a"    - 1. right window
"/home/smalmirror/value/b"    - 2. right window
"/home/smalmirror/value/c"    - 3. right window
"/home/smalmirror/value/d"    - 4. right window
"/home/smalmirror/label/a"    - 1. left window
"/home/smalmirror/label/b"    - 2. left window
"/home/smalmirror/label/c"    - 3. left window
"/home/smalmirror/label/d"    - 4. left window
the next following Windwo has a variable size
"/home/smalmirror/add"        - the bigger window with muteble lines at the lower area of the screen
"/home/smalmirror/addSize"    - change the size of the lower screen
