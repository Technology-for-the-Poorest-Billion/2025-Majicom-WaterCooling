To validate the results of the numerical python calculations for heat flow loss, a solidworks model was set up to recreate real world scenarios.

Deliverables:
* A validation and backup of numerical heat loss results to surroundings, for a tank held at 24C with outside surroundings at 29C.
* Simulations of convection flow for a variety of peltier or traditional coolant pipe methods

Mesh Dependancy Study
* A mesh dependancy / convergence study was conducted on the model to determine the optimal mesh size to use in modelling, as a compromise between accuracy and time spent on each mesh.
  ![WaterTankwWater-Thermal Flow Test-Image-1](https://github.com/user-attachments/assets/e8e47fb8-39bc-470c-a658-6d47428a5f3f)


Initial Results
* For a tank with top plate acting as a simulated peltier cooler having a set 24C condition, the net thermal condition (minus convection) looked like the below
  * net heat flux for this varied between 15 and 60 W, depending on if RMS (root mean squared) or average values of heat flux out were taken across the whole outer shell
