Basic concept
=============
First of all, it is really important to understand the definition of components and how it works together.

Tasc
^^^^
Tasc is a basic component of a scenario.
[example]

Terminus
^^^^^^^^
Terminus is defined as a human user or an intelligent agent that,
*has physical properties of a location and a bounding area
*has states (IntraState)
*is able to performs several actions
*is a subject of Instruction

Action
^^^^^^^^
Action is a dynamic behavior of Terminus that make changes of state or produce data. Some action has target of the action which is Terminus type.

Condition
^^^^^^^^^^^^
Condition is a deterministic criteria triggered by a range of State change.

Instruction
^^^^^^^^^^^^
Instruction transfers information that should be exactly announced to Terminus within a Tasc through Interfaces.

Context
^^^^^^^^^^^^
Context is a description of prerequisite. Currently supported as string.

Evaluation
^^^^^^^^^^^^
Evaluation is a component that quantify Terminus' performance by Measurement.
