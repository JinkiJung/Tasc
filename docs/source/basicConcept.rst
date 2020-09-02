Basic concept
=============
First of all, it is really important to understand the components and how it works together.
The use of Tasc assumes that the spatial parts of authoring, e.g., locating Terminuses and Interfaces in virtual environment, are done beforehand.

Tasc
^^^^
Tasc is a basic component and a single step of a scenario, following a simple syntax below::

  given:  prerequisite contexts
  when: condition that initiates Tasc
  who: intelligent terminus who performs Tasc
  do: action should be performed
  follow: instruction guiding who
  until: condition that terminates Tasc
  then: flow of scoring, feedback, and transition to next Tasc

Scenario
^^^^^^^^
Scenario is a container of Tasc components, a flow of those, and required resources.

Terminus
^^^^^^^^
Terminus is a object has physical properties of a location and a bounding area, and
  * has state
  * might represent spatial knowledge
  * might perform action
  * can be a subject of Instruction

Action
^^^^^^^^
Action is a dynamic behaviour of Terminus that produce State or data. Some action has *target* of the action which is Terminus type.
Action can be interpreted as a motor skill of a user to be performed at Tasc. The measurement for performance evaluation can be taken from Action.

Condition
^^^^^^^^^^^^
Condition is a deterministic criteria triggered by a range of State change.
For example *until* states the termination condition of Tasc.
To be more specific *until* performs as a trigger that the termination condition should be checked where the actual validation of the condition is performed by *then*.

Instruction
^^^^^^^^^^^^
Instruction transfers Information to Terminus through single or multiple Interfaces. A Tasc can have multiple instructions for the multimodal interaction.
It aims to guide a human user as a Terminus to accomplish the goal of the Tasc through multimodal interfaces.
For the case of Terminus as autonomous agent it can be used to inform its state or progress to human observers.

Context
^^^^^^^^^^^^
Context is a description of prerequisite. Currently supported as a list of strings.

Flow
^^^^^^^^^^^^
Flow is post processing of Tasc to control the flow afterward and consists of three parts: Evaluation, Feedback, and link to the next Tasc. Evaluation can be made through an equation with the measurements as variables resulting a float value.
Feedback then shows effects corresponding the score, which represents the user's performance through either a positive or negative way. Flow also provides link to the next Tasc based on the evaluation score.

Interface
^^^^^^^^^
Interface is a tool to represent Information with a sensory modality (such as visual, auditory, haptic, and others).
