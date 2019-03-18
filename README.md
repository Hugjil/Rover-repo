# Rover-repo

# Purpose
The purpose of this project is to simulate Mars Rover in real planet situation. Assume a rover named *"Mission Impossible"* arrives on Mars, and its mission is to find water which support life. 

# introduction
There are several States of Rover we need to take into consideration. 
* Rover initial state is **Wander**. 
* The sandstorm, which happens very often on Mars. If the *sandstorm is detected*, Rover should **Close Solar Panels** to aviod damage. Then, *reset* and back to **Wander**.  Evenmore, if the wind get stronger, the Rover should **Sleep**. Then,Rover will *reset* to **Close Solar Panels** or *mission start* to **Find Water** after sandstorm stop.
* If *Alien detected*, Rover should go to **Open Camera** state, emit event *camera set up* and the watch will capture this, turn camera running from false to true. By transition *record video* to **Close Camera**, then emit event *camera set up*, captured by watch to turn camera running from true to false. *send video back* will transit rRover to **Wander** state.
* Rover transits from **Wander** to **Find Water** by *mission start*, then transit to **Collect Water** by *found water*. Last transition is *mission complete* and back to **Wander** state. 

![qzDxjNf3TFSND%+EqJAr4Q_thumb_b5f](https://user-images.githubusercontent.com/12164360/54499655-6caaac00-48d1-11e9-897d-49cbab8d31b5.jpg)



# Goals
* The goal of this project is to stimulate the Mars Rover on 2D environment, and find water at location (154, 100). 
* The Rover will randomly walk one step each time on Mars' surface and record its location and report water status. 
* If there is no water, the Rover will record data index, location (x, y) and false for no water, then continue search. 
* If the Rover find water by luck, the Rover will record data index, location (x, y) and true for finding water, then exit the mission. 
* The Rover will emit event "camera set up" if alien is detected, and the watch will capture the event and set camera running status in true. 
* Alter recording, the Rover will emit another event "camera set up", and watch will capture this event and set camera running statue as false.  
* All the data stored by Rover will print out at final, and the last data should be the true for finding water.

# Milestone 
*1*. March 8th, start the project. decide to make car cruise problem. 

*2*. March 14th, change project to Mars Rover problem. 

*3*. March 15th, construct the States of Rover. Update the ReadMe file.

*4*. March 17th, collect the data that Rover gets.Implement the emit and watch event for Alien detected.

*5*. March 18th, turn in the final project with proper unit test.

# Resources
The resource used in this project are listed below:
* elma from professor's github. 
* robot from homework 7
* StateMachine from week 7 lecture. 
* reading from leetcode



