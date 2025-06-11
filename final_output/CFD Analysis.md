# CFD Analysis
Oscar Vitou

To validate the results of the numerical python calculations for heat flow loss, a solidworks model was set up to recreate real world scenarios with possibly greater accuracy.

## Deliverables:
* A validation and backup of numerical heat loss results to surroundings, for a tank held at 24C with outside surroundings at 29C.
* Simulations of convection flow for a variety of peltier or traditional coolant pipe methods.
* Humidity variation analysis of convective heat loss based on Tansanian weather conditions. 

## Static Analysis
### Static Mesh Dependancy Study
The first deliverable for this analysis method was a mesh dependancy  study, to determine the optimum mesh size to use as a compromise between accuracy and time spent on each mesh.

The results of the mesh dependancy study are seen below:

![RMS and Avg power loss against element size](https://github.com/user-attachments/assets/09491954-6c67-4027-b4e2-c160ffdb6ea8)

From this study, a mesh size of 130,000 elements was selected as the best compromise between simulation run-time and accuracy of results - reaching values within 2% of higher mesh sizes.

### Static Solidworks 2024 Analysis

The static heat flow simulation was able ot output heat power values for the tank when held at a temperature of 24C.

The results of the static static heat flow analysis are seen below.

![image](https://github.com/user-attachments/assets/9437ebff-5b66-46b2-a20e-98de5b394b3b)

| Analysis Type | Power demand | Peltier Power | Refrigerant Cycle Power |
| --- | --- | --- | --- |
| Static  | 8.7W  | 18-80W | 5.8W |

Solidworks 2024 has issues combining convection of fluids with heat transfer of materials additionally. Currently primary objective here is try and import the heat data from the static study and then run a convection simulation based off of that data.

**Convective Solidworks 2024 Analysis**

However, the overall steady state heat position that the tank will be aiming to achieve (regardless of gravity) will be that predicted in the static simulation, so should this not work data can still be gathered (though it should be noted that the data may be slightly inaccurate (unknown if over or under-esitmate)

![PeltierTop24Cooling](https://github.com/user-attachments/assets/ba0c682e-e84a-497d-86a9-a85c0aa002a2)

**Humidity Convective Analysis**

One feature of Solidworks Fluid Simulation is the ability to vary humidity. The humidity in Tansania varies throughout the year, with averages at a minima in 

**Final Results**


