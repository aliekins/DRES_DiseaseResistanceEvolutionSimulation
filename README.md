# Disease Resistance Evolution Simulation

## General idea:
The simulation would aim to model the long-term evolution of human populations in response to pandemics such as the Black Death (Black Plague), cholera pandemics, Spanish Flu, HIV/AIDS, Ebola and COVID-19. The focus is not only on disease spread but also on how genetic resistance and public health interventions shape survival outcomes over time. It would not be linear - one simulation over a long period of time of human history - experiencing all of the diseases, but instead "simulation per disease". By default, the population response (movement, medical response in form of vaccines) is limited to the "original state" the world was in - so for Black Death, less movement than today but also no effective medical response. These factors might be made adjustable, so that the user, even when simulating the Antonine Plague from 165 AD, could adapt it to the modern day response of the population.

To maintain scientific integrity, disease traits (transmission, lethality, incubation, etc.) would remain true to historical data, while the user can manipulate societal responses (like vaccination timing, quarantine compliance, sanitation improvements and possibly some others). The simulation might also evaluate intervention effectiveness in measurable formats - most likely percentage reduction in spread or mortality.

## Core parts of the project:
1. Organisms ("Human" population\s) - simplified of course
    agent-based simulation where each individual has: health, immunity strength, behavioral traits (quarantine obedience)
    reproduction would be asextual, in initial versions, so that trait/gene inheritance is straight forward
    if the organism lives certain duration of the simulation it reproduces and instantly dies (so there will be two of its copies left)
     if the organism is a survivor of certain disease, it may pass on genetic resistance (if it is possible for the given disease) over to their next generation
   
3. Diseases
    fixed properties based on real-world epidemiological data
    transmission and mortality evolve based on population density, movement, and medical responses
   
5. Simulation Logic 
     C# engine runs disease spread calculations, intervention effects, and genetic shifts (basically anything highly computational)
   
7. UI & visualization 
    most likely done with Unity
    agent-based visualization (infected individuals change color, ones with high immunity have a certain trait - line over them, hat or something which would distinguish them)
    user may control public health policies (vaccine rollout, social distancing, travel restrictions)
    may include: graphs and data displays comparing simulated outcomes with historical records
