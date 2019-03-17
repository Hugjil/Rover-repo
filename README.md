# Rover-repo

The purpose of this project is to simulate Mars Rover in real situation. Assume a rover named *"Mission Impossible"* arrives on Mars, and its mission is to find water which support life. 

There are several States we need to take into consideration. 
* Rover initial state is **Wander**, 
* The sandstorm, which happens very often. If the *sandstorm is detected*, Rover should **Close Solar Panels** to aviod damage. Then, *reset* and back to **Wander**.  Evenmore, if the wind get stronger, the Rover should **Sleep**. Then, *reset* to **Close Solar Panels** or *mission start* to **Find Water** after sandstorm stop.

*If *Alien detected*, Rover should go to **Open Camera** state, emit event *camera set up* and the watch will capture this, turn camera running from false to true. By transition *record video* to **Close Camera**, then emit event *camera set up*, captured by watch to turn camera running from true to false. *send video back* will transit rRover to **Wander** state.

*Rover transits from **Wander** to **Find Water** by *mission start*, then transit to **Collect Water** by *found water*. Last transition is *mission complete* and back to **Wander** state. 

* The **temperature** decrease 0.6 Celsius by every 100 meters elevation gain. 
* **Fehn wind** flows from Rockey Mountain to Great Plain, slow down the speed of the car. 
* **changeing gear** of the car, which will also change its speed.


Milestone: 
1. March 8th, start the project. decide to make Mars Rover problem. 
2. March 14th, build emla environment. 
3. March 18th, construct the States of Rover.
4. March 20th, collect the data that Rover gets.
5. March 22th, turn in the final project with proper unit test.

The success of this project is to find water at exact location (154, 100),  the rover will randomly walk around Mars' surface and record its location and water status. If there is no water, the Rover will record data index, location (x, y) and false for no water, then continue search. If the Rover find water by luck, the Rover will record data index, location (x, y) and true for no water, then exit the mission.  all the data stored by Rover will print out at final, and the last data should be the true for finding water.

The resource I am gonna use is elma, robot, and StateMachine. 


