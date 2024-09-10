# Power Usage Simulation System
# Author: Gerardo Gutierrez
## Description
Java application to simulate power consumption management for a building, focusing on
efficient power usage of regular and smart appliances.

## Languages Used
* Java

## Environments Used
* Windows 10

## Program Demo Video 
[Watch the Demo Video](https://www.youtube.com/watch?v=YourVideoID)

## Program walk-through
Power Simulation Instructions

1. Add your txt or csv file which holds all of the appliances and their info, into the project folder. This file should have all the appliance details separated by commas in the following format:
   `LocationID,ApplianceDescription,OnWattage,ProbabilityOfBeingOn,isSmart (represented by true or false), percentPowerReduction (double between zero and one)`
   (See [`app.txt`](app.txt) file in the repository folder for an example)

2. Add the [`Main.java`](powerGridSimulation/Main.java), [`Appliance.java`](powerGridSimulation/Appliance.java), and [`Location.java`](powerGridSimulation/Location.java) files to the same package folder.

3. Run [`Main.java`](powerGridSimulation/Main.java).

4. Enter the inputs requested by the program: allowed wattage (int), timesteps (int), and the name of the input file.

5. The user is prompted to select an option from the menu. Follow the directions on screen and select your desired option.

6. When the simulation is complete there will be two outputs:
   - **OUTPUT TO SCREEN**: Total appliances set to low per timestep, total browned out locations per timestep, total affected locations per timestep, max affected location of the entire simulation
   - **FILE OUTPUT**: `output.txt` file containing the appliances affected per timestep, the locations affected per timestep
