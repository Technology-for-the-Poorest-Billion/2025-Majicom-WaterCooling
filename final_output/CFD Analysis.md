# CFD Analysis
Oscar Vitou

To validate the results of the numerical python calculations for heat flow loss, a solidworks model was set up to recreate real world scenarios with possibly greater accuracy.

## Deliverables:
* A validation and backup of numerical heat loss results to surroundings, for a tank held at 24C with outside surroundings at 29C.
* Simulations of convection flow for a variety of peltier or traditional coolant pipe methods.
* 

## Static Analysis
### Static Mesh Dependancy Study
The first deliverable for this analysis method was a mesh dependancy  study, to determine the optimum mesh size to use as a compromise between accuracy and time spent on each mesh.
### Static Solidworks 2024 Analysis

The static heat flow simulation was able ot output heat power values for the tank when held at a temperature of 24C.

The results of the static mesh dependancy study are seen below.

  ![WaterTankwWater-Thermal Flow Test-Image-1](https://github.com/user-attachments/assets/e8e47fb8-39bc-470c-a658-6d47428a5f3f)

| Analysis Type | Power demand | Peltier Power | Refridgerant Cycle Power |
| ------------- | ------------- | --- | --- |
| Static  | 8.7W  | 18-80W | 5.8W |

Solidworks 2024 has issues combining convection of fluids with heat transfer of materials additionally. Currently primary objective here is try and import the heat data from the static study and then run a convection simulation based off of that data.

**Convective Solidworks 2024 Analysis**

However, the overall steady state heat position that the tank will be aiming to achieve (regardless of gravity) will be that predicted in the static simulation, so should this not work data can still be gathered (though it should be noted that the data may be slightly inaccurate (unknown if over or under-esitmate)

![PeltierTop24Cooling](https://github.com/user-attachments/assets/ba0c682e-e84a-497d-86a9-a85c0aa002a2)

**Humidity Convective Analysis**

One feature of Solidworks Fluid Simulation is the ability to vary humidity. The humidity in Tansania varies throughout the year, with averages at a minima in 

**Final Results**


