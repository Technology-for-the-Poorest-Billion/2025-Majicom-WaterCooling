# Conclusions 

The final conclusions of our investigation can be seen below.

## Analysis results


| Cooling method  | Power demand | Complexity | Cost | Problems
| ------------- | ------------- | ----|----|---- |
| Cooling on demand  | 200 W  | Peltier cell - small complexity | small| Peltier cell effficiency test|
| Cooling the whole tank  | 250 W | Refrigerant cycle - high complexity| medium | Reduced efficiency of passive cooling
| Cooling with the mains water | 0 | Expensive heat exchanger - medium complexity | very high| Large heat exchanger needed |
| Cooling a smaller tank | 70 W | Refrigerant cycle and a smaller tank - very high complexity | high | Need for many components|

The results as seen in the table above show the conclusions from the thermodynamic analysis. Below is a short description about each fo the solutions and under what conditions would it be suitable.

### Cooling on demand

This option would consist of a peltier cell and a heat exchanger placed shortly before the dispensing point in the machine.
This option would be simple to implement, and relatively cheap. However it comes with a hefty energetical price tag.
Some suggestions that would make this option more viable:
 - higher cost of cold water - this would act to reduce the number of people regularly buying it and hence reduce the average power demand.
 - use of mains power - it is possible to run this system mostly on solar panels unless in times of greater demand. Should teh demand slowly drain the battey, it could be recharged from the mains power supply.
This would allow power independence, while preserving access to cold water in varying demand

### Cooling the whole tank

This option would consist of a cyclic refrigerant cycle through which water from the tank is constantly pumped.
This is not too difficult to implement, however it would reduce the water temperature for all user, no matter
whether they want it or not. Secondly, this would have a negative impact on passive cooling, which seems to be the most efficient cooling option.
For these reasons, unless passive cooling is not applicable, this option is not advised.

### Cooling with mains water

This option would consist of a heat exchanger between mains water and dispensed water in order to leverage the coldness of the water supply.


### Cooling a smaller tank

This is an approach used often in commercial cold water dispenser. This would include fitting a secondary smaller water tank,
which would be cooled constantly with a cyclic cooler. This would be the most energy efficient option, however
also the most complex to implement. This option would be the best one if the power limitation prove to be impossible to overcome. 

In this case we recommend to purchase a commercial cold water dispenser to reverse engineer the solutions used there. 

### Solidworks 2024 Validation

To further validate the numerical analysos, solidworks simulations were conducted to validate heat flow power requirements to maintain temperature.
![PeltierTop24Cooling](https://github.com/user-attachments/assets/9d23ece7-136b-449f-b6f5-6b737a1007f3)

