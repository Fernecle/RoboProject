# RoboProject

Requirements per software module as per described in the project booklet.

Robot model and physics simulations
1. Uses an even floor.
2. All modules and obstacles are solid objects.
3. The size of objects is defined in normalized grid units.
4. Modules can't fly nor jump.
5. Obstacles can't move or be moved.
6. Robots always move one complete grid unit per unit simulation time step.
7. Robots can slide in x- and y-direction through translation on either the floor or other modules.
8. Robots can slide in z-direction through translation alongside other modules or obstacles.
9. Robots can only move in one direction per time unit so no diagonal movements.
10. Robots can only move to a new grid unit if it's not going to be occupied in the NEXT time unit.
11. If a robot is moving over the edge of another module or obstacle it attaches to the side (no gravity).
12. A robot can not stay connected with only it's top surface (no hanging).
13. A robot can slide underneath another robot.
14. A robot can only move its own weight. It cannot carry other modules.

AI and Control
1. Seperate module so it can be replaced later on.
2. Research AI algorithms and explain those in presentation.
3. Provide an implementation at least for a simple AI based on sequential movements of single robotic modules.

4. AI should follow these steps:
  1. Select a robot from the start configuration that is free to move.
  2. Move this robot all the way to a seat in the target configuration while avoiding dead-locks or blocking any seats in the target configuration.
  3. Do not move through obstacles.
  4. The AI has to respect the "Robot model and physics" rules.
  5. Continue moving robots until all free seats in the target configuration are occupied by robots.

5. Test the AI with self-chosen configurations.
6. Provide measurement for how many computational steps your AI algorithm takes (more of this in booklet).
7. Provide measurement for how many discrete simulation time steps your reconfiguration algorithm requires (more of this in booklet).
8. Provide measurements to show how your algorithm scales with respect to
the number of modules in the target configuration.
9. Demonstrate at least one set of configurations that your algorithm cannot
solve and provide a meaningful explanation why this is the case.
