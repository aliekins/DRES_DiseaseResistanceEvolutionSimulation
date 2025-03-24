# Disease Resistance Evolution Simulation

## Main focus?
_The main objective of this project is to develop a biologically grounded, agent-based simulation of disease resistance evolution in human populations, enhanced with an interactive and visually engaging interface to support intuitive exploration of historical and hypothetical pandemics._

## General idea:
(still not final formulation)<br>
_The objective of this thesis is to design and implement an agent-based simulation that models the evolution of disease resistance in human populations using evolutionary algorithms and reinforcement learning. The simulation will be centered around historically accurate disease scenarios, such as the Black Death, cholera pandemics, Spanish Flu, HIV/AIDS, Ebola, and COVID-19. Human agents will be represented as simplified organisms with basic health, immunity, and behavioral traits. Disease properties will remain fixed based on real-world epidemiological data, while user-controlled public health interventions will influence population outcomes. The system will be implemented with a C# computational core and visualized through Unity, offering an interactive interface for observing disease spread, immunity development, and the long-term genetic adaptation of populations. The aim is to explore how pandemics shape evolutionary outcomes and to evaluate the conditions under which genetic resistance emerges and persists in affected populations._

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


## Current path:
**Phase 1** of the project - biological foundation 
For the next ~6 months the goal is to build the core simulation engine
 - Modeling key diseases accurately using real-world epidemiological parameters.
 - Implementing simplified agent-based human populations with health, immunity, and behavior traits.
 - Including evolutionary inheritance and disease resistance logic.
 - Validating basic results
What should be there in the end:
 - Working simulation with real diseases.
 - Console or basic UI with sliders and stats.
 - Scientific justification for biological simplifications.


**Phase 2** of the project - visual expansion
 - Implementing visual UI and interaction layer in Unity.
 - Using human-like agents, animations, and visual indicators for their attributes
 - Adding graphs, timeline progression, and feedback visualization.
What should be there in the end:
 - Interactive GUI with toggleable scenarios.
 - Scenario replay system and comparison tools.
