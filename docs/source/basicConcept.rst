Basic concept
=============
First of all, it is really important to understand the definition of components and how it works together.

Tasc
^^^^
Tasc is a basic component and a single step of a scenario, following a simple syntax below::

  given: some contexts
  when: condition that initiates Tasc
  who: intelligent terminus who performs Tasc
  do: action should be performed
  follow: instruction guiding who
  before: condition that terminates Tasc
  then: scoring, corresponding feedback, and moving on to next Tasc

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
Action is a dynamic behavior of Terminus that produce State or data. Some action has *target* of the action which is Terminus type.
Action can be interpreted as a motor skill of a user to be performed at Tasc. The measurement for performance evaluation can be taken from Action.

Condition
^^^^^^^^^^^^
Condition is a deterministic criteria triggered by a range of State change. In the context, *before* states the termination condition of Tasc, but not the goal.
Evaluation on the goal achievement will be done in *then*.

Instruction
^^^^^^^^^^^^
Instruction transfers information that should be exactly announced to Terminus within a Tasc through Interfaces.
Instruction can be used to inform what happens within the Tasc execution.

Context
^^^^^^^^^^^^
Context is a description of prerequisite. Currently supported as string.

Flow
^^^^^^^^^^^^
Flow is post processing of Tasc to control the flow afterward and consists of three parts: Evaluation, Feedback, and link to the next Tasc. Evaluation can be made through an equation with the measurements as variables resulting a float value.
Feedback then shows effects corresponding the score, which represents the user's performance through either a positive or negative way. Flow also provides link to the next Tasc based on the evaluation score.
