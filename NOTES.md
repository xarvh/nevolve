
Commands:
  - Thrust angle, force
  - RotateFormation torque
  - A Trigger
  - B Trigger


Player Ship:
- It has a unique Core part: if it is destroyed, the ship is destroyed
- The Core is the only part that doesn't need to be attached anywhere
- The Core produces a small amount of Energy
- Energy can be used to Thrust and Regenerate parts.
- Regeneration happens automatically, using all the Energy available.
- All new Ships begin play with just a small Core, and slowly develop the other body parts
- If not enough Energy is available, Thurst may be impaired.
- All other parts are regenerated according to the Genome, and have different types and sizes and orientation.
- When parts collide with anything, they maytake damage
- The parts can be
  * Core (one and only one)
  * Thruster (for the player, they are omnidirectional)
  * Generator (they produce Energy)
  * Accumulator (they store Energy. May explode violently when destroyed)
  * Armor (does nothing, but it's sturdy and relatively light)
  * Disconnector A (when player presses A, it breaks shooting children and parent apart)
  * Disconnector B (when player presses B, it breaks shooting children and parent apart)
  ? Reproduction part (using available Energy builds up X where X is what is used to continue the game if the current ship is destroyed)
  * Connector part (modifies angle and distance of the Ship inside the formation according to its position relative to the Core)


Generations:
- Ships are always spawned in batches, called Generations.
- When the last Ship of a Generation is destroyed, a new Generation of Ships are spawned, depending on how much X was produced by the previous generation.
- There is a maximum number of ships in the new Generation, any excess X is used to push the new Ship's development forward.
- The Ships stay in formation and execute the same commands.


Evo-Devo:
- Many cells connected to each other
? How are new cells built?
- Each cell has different concentration of a set of substances
- Concentrations diffuse into nearby cells
- Each substance will bind to a specific genetic sequence
? Activation vs repression? of specific genetic sequences that affect local concentrations


Cells geometry and appearance
- A Ship's body is made of Cells
- Each Cell is modelled as two triangles: each side of the triangle represents a linear constraint on the cell's shape
- A Cell splits along the line between the two vertexes that are not shared between the two triangles
- Each triangle has forces acting upon it that prevent it from having obtuse angles
- A Cell's rendering does not have to match the Cell geometrical model





