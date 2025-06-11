# Conclusions 

The final conclusions of our investigation can be seen below. All the numbers and calculations shown in this file are explained in `Active cooling model.ipynb`

## Analysis results


| Cooling method  | Power demand | Complexity | Cost | Problems
| ------------- | ------------- | ----|----|---- |
| Cooling on demand  | 200 W  | Peltier cell - medium complexity | small| Peltier cell effficiency test|
| Cooling the whole tank  | 250 W | Refrigerant cycle - high complexity| medium | Reduced efficiency of passive cooling
| Cooling with the mains water | 0 W | Expensive heat exchanger - medium complexity | very high| Large heat exchanger needed |
| Cooling a smaller tank | 70 W | Refrigerant cycle and a smaller tank - high complexity | high | Need for many components|

The results as seen in the table above show the conclusions from the thermodynamic analysis. Below is a short description of each of the solutions.

### Cooling on demand

This option would consist of a peltier cell and a heat exchanger placed shortly before the dispensing point in the machine.
This option would be simple to implement, and relatively cheap. However it comes with a hefty energetical price tag.
Some suggestions that would make this option more viable:
 - higher cost of cold water - this would act to reduce the number of people regularly buying it and hence reduce the average power demand.
 - use of mains power - it is possible to run this system mostly on solar panels unless in times of greater demand. Should the demand slowly drain the battery, it could be recharged from the mains power supply.
This would allow power independence, while preserving access to cold water in varying demand.

However, the efficiency of Peltier cells under realistic conditions is not certain to be high enough to provide enough cooling power. The test conducted failed to achieve high enough efficiency to act as a proof of concept. There are several important difficulties connected to using Peltier cells: expensive heat exchangers, low efficiency and high current necessary. For these reasons, among others as discussed before, it was determined that further development should be focused on refrigerant cycles. 

### Cooling the whole tank

This option would consist of a cyclic refrigerant cycle through which water from the tank is constantly pumped.
This is not too difficult to implement, however it would reduce the water temperature for all user, no matter
whether they want it or not. Secondly, this would have a negative impact on passive cooling, which seems to be the most efficient cooling option.
For these reasons, unless passive cooling is not possible, cooling a smaller tank should be preferred.

### Cooling with mains water

This still holds potential, as research suggests that the mains water would be up to 10 degrees cooler than our cold tank temperature, depending on time of year, degree of cooling achieved in the tank, and pipe insulation, and the volume of water available is limitless and cheap. The problem however is that the low temperature difference means that large and expensive heat exchangers are required. The other issue is that at some points the mains water will be similar in temperature to the tank, or possibly warmer, meaning that some sort of temperature detection and diversion system would need to be included into the solution, adding additional complexity, failure points and energy sinks. Overall, this avenue does not hold too much potential if looking for a budget solution, but I do think that in future additions, some mains cooling elements could be a low power way to get considerable cooling, subject to heat exchangers available.


### Cooling a smaller tank

This is an approach used often in commercial cold water dispenser. This would include fitting a secondary smaller water tank,
which would be cooled constantly with a cyclic cooler. This would be the most energy efficient option.
The calculated power of 70 Watts may be optimistic.
It is based on the assumption that just 30% of customers would be willing to pay extra for cooled water.
Additionally, it assumes quite a high coefficient of performance of 1.5.
Nevertheless, these numbers are in range of what commerical systems use and should be possible to reproduce. 

Hence, as the next step to this experiment we suggest the following:
- purchase a commercial cold water dispenser to reverse-engineer the solutions used there.
- purchase a DIY refrigerant module and measure its performance, to gain a realistic estimate of the performance
- try to assemble the cheapest refrigeration cycle possible, to gauge more closely the costs involved

We believe that these steps should ensure high performance and low cost of the future system. Price of about £100 should be achievable. Additionally, this offers the possibility of repurposing old refrigerant module, thrown out in more developed countries, but containing useful components in less developed countries. This will also act as to further reduce the waste problem in African countries, while helping the local economy. such a solution is worth further research and again highlights the usefulness of reverse-engineering commercial solutions.

### Results validity

These recommendations are based on models and research, which can be found on this github page. much of it can be found in the `Active cooling model.ipynb`, but the `interim` folder also contains some other useful analyses. 

More specifically, active cooling model begins with a simple thermodynamic analysis, but later the models were validated using more complicated models, experiment results and a Solidworks heat losses simulation.

## Final recommendation

From the data available, several conclusions can be drawn:

 - the only option that would fit into current energy budget is cooling a smaller tank. This is an option done commercially and such system could be retrofitted and reverse engineered from existing systems.
 - Despite their complexity, refrigerant cycles offer more efficient cooling and would be likely more suitable than Peltier cells
 - Cooling a whole tank is an option especially in the wet season. This would require larger solar panel area and may interfere with passive cooling.

There are several possible next steps from this research. The clearest path to successful implementation is purchasing a simple cyclic cooling module and/or a commercial water cooling system. It was determined that passive cooling approaches hold more promise in delivering large cooling at smaller power, so they should be prioritised. The active cooling approaches can be then fitted on top of passive cooling. 
Nevertheless, keeping in mind that the power usage of refrigeration modules is actually not as prohibitively high as previously thought, we advise that this area should be tested and implemented.
