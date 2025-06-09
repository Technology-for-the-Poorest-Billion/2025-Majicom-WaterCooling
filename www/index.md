---
title: About Our Project
---

# Chilled Water for Majicom Kiosks

## Introduction

This story starts with **Majicom**, a company that provides purified drinking water kiosks in Tanzania that run on low amounts of power sourced from solar panels. Majicom is a not-for-profit organisation aiming to create a cheaper and more eco-friendly source of drinking water in urban areas.

Chilled water has been shown—through user surveys—to be a desirable feature, and that’s where we come in. Our challenge: **advise Majicom on how to cool the water by 5–10°C from ambient**, while still meeting constraints on power, space, and sanitation.

![Majicom Kiosk](images/kiosk.jpg)

## Active and Passive Cooling

When it comes to water cooling methods, we identified two main approaches:

- **Active cooling** – using a heat pump (like the refrigerant cycle used in fridges).
- **Passive cooling** – using **evaporative cooling**, where water absorbs heat as it evaporates into surrounding air.

With a large team size and fairly independent cooling solutions, we split into sub-teams. Our team focused on **active cooling**.

## Tank Sizing and Insulation

![Tank Sizing Calcs](images/sizing-calcs.jpg)

### Objective

Determine whether the main energy constraint is due to:
- Heat lost from the water tank, or
- Energy needed to chill water dispensed during peak times.

### Work Done

- Rough calculations of cooling power needed to serve customers during peak hours.
- Estimating tank heat loss from conduction/convection, assuming added insulation.

### Conclusions

If the tank is insulated, heat loss becomes relatively minor compared to the cooling power required during peak demand. Therefore, **focus should be on water throughput cooling**, not tank losses.

## Whole System Modelling

![System Modelling Graphs](images/system-modelling.png)

### Objective

[Insert objective]

### Work Done

[Insert work done]

### Conclusions

[Insert conclusions]

## CFD (Computational Fluid Dynamics)

![CFD Results](images/cfd-results.png)

### Objective

[Insert objective]

### Work Done

[Insert work done]

### Conclusions

[Insert conclusions]

## Tap Water Cooling

![Pipe Length Graph](images/pipe-length-graph.png)

### Objective

Investigate the feasibility of using cold **incoming tap water** as an auxiliary cooling source.

### Work Done

- Studied tap vs ambient temperatures in tropical regions.
- Assessed feasibility of heat exchangers transferring heat from tank to colder tap supply.
- Explored passive methods like direct pipe immersion.

### Conclusions

Tap water in Tanzania is generally cooler than the desired tank temp, offering potential for pre-cooling. However, small temperature differences (~5°C) mean **large and costly heat exchangers** would be needed. Simpler solutions (e.g., pipe coiling) were also found **too expensive** for meaningful cooling.

## Testing Peltier Cell Cooling

![Peltier Experimental Setup](images/peltier-test.jpg)

### Objective

Can water be cooled **on-demand** during dispensing using Peltier cells?

### Work Done

- Built a circuit using PC cooling parts to test real-world Peltier performance.
- Transferred heat from water → Peltier → air.

### Conclusions

**Peltier cells were too inefficient** to cool water at required rates. To be viable, they would need **additional heat exchangers and high-power fans**, making them too expensive and complex for this application.

## Final Conclusions

### Our Recommendation to Majicom

From our investigations, several clear conclusions were drawn:

- The **only viable option within the existing energy budget** is to cool **smaller tanks**, a solution used commercially and retrofittable to existing kiosks.
- Despite their complexity, **refrigerant-based cooling systems** are significantly more efficient and more appropriate than Peltier-based options.
- **Cooling a whole tank** is viable, especially in the **wet season**, but would require **larger solar panels** and may interfere with passive methods.

## Next Steps

The clearest path to successful implementation involves:

- Purchasing or building a **simple, compact refrigerant-based cooling module**.
- Investigating partnerships with **commercial water chilling system manufacturers**.
- Continuing research into **passive enhancements**, like insulation and spectrally selective coatings.

