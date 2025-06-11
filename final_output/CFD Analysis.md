# CFD Analysis
>Oscar Vitou

To validate the results of the numerical python calculations for heat flow loss, a solidworks model was set up to recreate real world scenarios with possibly greater accuracy.

## Deliverables:
* A validation and backup of numerical heat loss results to surroundings, for a tank held at 24C with outside surroundings at 29C.
* Simulations of convection flow for a variety of peltier or traditional coolant pipe methods.
* Humidity variation analysis of convective heat loss based on Tansanian weather conditions. 

## Static Results
### Static Mesh Dependancy Study
The first deliverable for this analysis method was a mesh dependancy  study, to determine the optimum mesh size to use as a compromise between accuracy and time spent on each mesh.

The results of the mesh dependancy study are seen below:

![RMS and Avg power loss against element size](https://github.com/user-attachments/assets/09491954-6c67-4027-b4e2-c160ffdb6ea8)

From this study, a mesh size of 130,000 elements was selected as the best compromise between simulation run-time and accuracy of results - reaching values within 2% of higher mesh sizes.

### Static Solidworks 2024 Results

The static heat flow simulation was able ot output heat power values for the tank when held at a temperature of 24C.

The results of the static static heat flow analysis are seen below:

![image](https://github.com/user-attachments/assets/9437ebff-5b66-46b2-a20e-98de5b394b3b)

| Analysis Type | Power demand | Peltier Power | Refrigerant Cycle Power |
| --- | --- | --- | --- |
| Static  | 16.8W  | 34-169W | 11.2W |

## Convective Results

### Convective Mesh Dependancy Study

A mesh dependancy study was conducted using the Solidworks 2024 Fluid Simulation add-on, allowing for an optimum compromise between simulation run-time and computational accuracuy to be selected.
The results of the mesh dependancy study can be received below:
![Power Loss against Element Size](https://github.com/user-attachments/assets/c37bd8de-58bb-4a9a-b8d6-1f4b5138073a)

It was found that the maximum mesh element size of approximately 40,000 cells was able to produce the most accurate results in a reasonable time-frame - therefore this rough cell count was carried forward for all further convective studies.

### Convective Solidworks 2024 Results

A convective analysis was conducted using Solidworks Fluid Simulation analysis, with boundary conditions setting the 24C condition on the interior wall, allowing for internal rough heat transition to be visualised in addition to external heat flow transfer in the surrounding air.

Results for this study can be seen below, and a visualisation of the convection flow in the air surrounding the tank is seen below.

![24CConvective50%Humidity_1](https://github.com/user-attachments/assets/f1e0c29b-bbba-49d0-869f-e46bdd291041)

| Analysis Type | Power demand | Peltier Power | Refrigerant Cycle Power |
| --- | --- | --- | --- |
| Convective | 17.4W  | 35-174W | 11.6W |

## Analysis

The results for both static heat flow calculations and convective solutions are to within <2% of each other. These results also further support the results found in the numerical analysis, further supporting their validity and accuracy. It is worth noting that in the convective analysis, a static image of the heat conduction within the tank is observed - this is a static condition and a limitation of Solidworks 2024 Fluid Simulation: only one of external or internal analyses can be conducted at any one time. However, it was found through internal experimentation that the convective effects outside of the tank were far more significant than internal flow characteristics due to temperature variation.

**Humidity Convective Analysis**

One feature of Solidworks Fluid Simulation is the ability to vary humidity. The humidity in Tansania varies throughout the year, with averages at a minima in 

**Final Results**


