# Sprint 1 Page

Here the Plan is to add the Autorunning Mechanic to a level in Unreal Engine that sets a 3D actor to run contionously towards a set player or location.

I have achieved this by using a Blackboard task i named "RunInPlace". Attached to a selector node. AI Perception "Sight" allows the AI to find the Blackboard Key "Target Location". The AI Character can see the player start actor and move towards it continously. 
<img width="462" height="846" alt="runinplace" src="https://github.com/user-attachments/assets/885e49d8-4b8e-477d-8698-9b60490ec8aa" />


This blueprint runs the behaviour tree firing off the above Task and tells the AI to get all Actors of class, in this case its the first player start actor, being integer "0" , getting the controlled actor "AI Character" and telling it to move to Player start location. 
<img width="857" height="218" alt="ai controller" src="https://github.com/user-attachments/assets/12c14950-92a9-4f5a-83e7-2f42cf7695f5" />



This Blueprint tells the AI Character to stop moving but play its running animation, As i have set the movenment boundaries of the AI to a small area, and the player start actor "Target Location" is located outside the boundaries, the selector fails and restarts continuously, achieving the desired running in place effect.
<img width="1005" height="339" alt="BehaviourtreeTask" src="https://github.com/user-attachments/assets/de6b5cde-34c6-440c-8c2b-7fc77b32c9f1" />


Here you can see a picture of the world as the AI character tries to reach the Target Location
<img width="735" height="526" alt="sprint1" src="https://github.com/user-attachments/assets/dc115d88-ced2-4fc8-af35-877836110cbf" />
