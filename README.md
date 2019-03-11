# cruiseControl-repo

The purpose of this project is to build a model of car cruise in real situation. Assume two cars drives from Kansas city to our mile high city Denver, the elevation change from 277 meter (909 feet) to 1609 meter (1 mile). The distance from Kansas city to Denver is 970 km. 

There are several conditions we need to take into consideration. 
* The **oxygen** content decrease due to the increases of elevation. Without rich oxygen, combustion engine cannot burn gasoline totally.
* The **temperature** decrease 0.6 Celsius by every 100 meters elevation gain. 
* **Fehn wind** flows from Rockey Mountain to Great Plain, slow down the speed of the car. 
* **changeing gear** of the car, which will also change its speed.


Milestone: 
1. March 8th, start the project. decide to make car cruise race problem. 
2. March 14th, build two cars using elma. 
3. March 18th, build the manager for two cars.
4. March 20th, build emit and watch for two cars.
5. March 22th, turn in the final project with proper unit test.

The success of this project is determined by our cars, the car with higher gear moves faster, and comes to the destination first at end. When the car emit the change gear command, the watch will capiture the command and speed up the car. 
The resource I am gonna use is elma, robot, and car cruise control. 
