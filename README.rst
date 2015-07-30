################################################################################
Very Simple Alife Simulator
################################################################################

*Very simple artificial life simulator to show the evolution of (somewhat) intelligent behavior.*

The simulated creatures live in a rectangular grid, and there are discrete time steps. The types and properties of all creatures are fixed, but their behavior is variable and evolves randomly. Intelligent behavior should emerge through random selection. There are three types of creatures: plants, herbivores and carnivores. Additionally there can be obstacles in the grid.

**This project is in early alpha stage, there is no code yet.**


The Creatures
================================================================================

There are three types of creatures: plants, herbivores and carnivores. Additionally there are obstacles.

Plants
--------------------------------------------------------------------------------

Plants appear randomly at a certain rate during the simulation. The region where plants appear can be restricted to a rectangular area, so that intelligent behavior can be more easily viewed. Plants can not move, and die after a certain time.

By eating plants herbivores gain a certain amount of energy. Plants are the source of energy for all life in the simulation.

Herbivores
--------------------------------------------------------------------------------

Herbivores eat plants to gain energy. They lose a certain amount of energy at each time step. When their energy reaches zero they die.

Herbivores can see, smell, turn and move. Their behavior is controlled by their brains.

Carnivores
--------------------------------------------------------------------------------

Carnivores eat herbivores to gain energy. Like herbivores they lose a certain amount of energy at each time step. When their energy reaches zero they die.

Carnivores can see, smell, turn and move. Their behavior is controlled by their brains.

Obstacles
--------------------------------------------------------------------------------

Obstacles are placed in the grid prior to the simulation. Animals can not cross obstacles.


Visual Sense
================================================================================

All animals can view one or more fields straight ahead. The visual sense tells the distance of the viewed object, but not the exact direction. The view covers a triangular area, 45° wide. By turning 8 times the animal can look around.


Smell
================================================================================

All animals have a sense of smell, which is undirected (covers 360°) but tells the approximate distance. 
