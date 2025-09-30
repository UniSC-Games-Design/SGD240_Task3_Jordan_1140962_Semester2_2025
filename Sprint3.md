# Sprint 3 page

## The plan here is to add the code to allow the AI Character to respond to the grenades being fired at them.



I will be using the Projectile system from Sprint 2 

Initally we will be testing this with just 1 type of grenade and the AI will respond by attempting to evade the grenade by turning away 


Firstly I will be using the AI Perception system so set up my AI Characters vison, so they can see the projectiles being fired.


Add AISense_Sight to the perception system and add a AIPerceptionStimuliSource Component to the projectile blueprint.


Set up a new Blackboard Key for the decision making


Add a selector branch to assign high priority to assess incoming projectiles


Add a new "Dodge Task" that lets the AI Character Dodge/ Duck/ Jump over projectiles.


Add more nodes to the Blackboard to check the projectiles speed and velocity to allow the AI to calculate interception for the "Dodge Task"
