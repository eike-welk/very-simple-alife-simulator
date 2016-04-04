################################################################################
Very Simple Alife Simulator
################################################################################

*Very simple artificial life simulator to show the evolution of (somewhat) intelligent behavior.*

The simulated creatures live in a rectangular grid, and there are discrete time steps. The types and properties of all creatures are fixed, but their behavior is variable and evolves randomly. Intelligent behavior should emerge through random selection. There are three types of creatures: plants, herbivores and carnivores. Additionally there can be obstacles in the grid.

**This project is in early alpha stage, there is no code yet.**


Creatures and Other Simulated Objects
================================================================================

There are three types of creatures: plants, herbivores and carnivores. Additionally there are obstacles.

Plants
--------------------------------------------------------------------------------

Plants appear randomly at a certain rate during the simulation. The region where plants appear can be restricted to a rectangular area, so that intelligent behavior can be more easily viewed. Plants can not move, and die after a certain time.

By eating plants herbivores gain a certain amount of energy. Plants are the source of energy for all life in the simulation.


Animals
--------------------------------------------------------------------------------

Animals are the main subject of the simulation. They can see, smell, turn, move, eat and procreate. Their behavior is controlled by their brains.

Animals must eat to gain energy. They loose energy with each step of time, and die when their energy drops to zero. When an animal's energy reaches a certain level they procreate.

There are two types of animals:

Herbivores: 
    Herbivores eat plants to gain energy. 

Carnivores:
    Carnivores eat herbivores to gain energy. 


Obstacles
--------------------------------------------------------------------------------

Obstacles are placed in the grid prior to the simulation. Animals can not cross obstacles.


Brain
================================================================================

All animals have a brain, that controls their actions. The brain contains a short program, that is modified randomly when the animal procreates.

The brain contains a series of "if" statements that are all evaluated at each time step. 

Visual Sense
--------------------------------------------------------------------------------

All animals can view one or more fields straight ahead. The visual sense tells the distance of the viewed object, but not the (exact) direction. The view covers a triangular area, 45° wide. By turning 8 times the animal can look around.

Smell
--------------------------------------------------------------------------------

All animals have a sense of smell, that tells them the distance and number of other creatures, but not the direction. 

Pain
--------------------------------------------------------------------------------

All animals a have a sense of pain, that tells them the direction and strength of an attack against them.
