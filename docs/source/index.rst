.. Tasc documentation master file, created by
   sphinx-quickstart on Fri Feb 14 10:08:33 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

==============================
Tasc |version| documentation
==============================
**Tasc** is a high-level script for representing tasks and its consequences, as its ambitious nickname is *new wheel*.
Tasc can represent a procedure of task, scenario by indicating which information needs to be transferred, and how the performance of the actor can be evaluated by chosen measurements.
The use of Tasc will radically reduce the time and cost of implementing a scenario when it comes to development of an executable program of VR/AR or simulation.
The scope of Tasc is only for modelling of scenario. It's execution is dependent to the engine that compiles the script. Same Tasc can be differently interpreted by different dependency.
Tasc enables more accurate communication of client and developer through syntax in implementation.

Primary usage of Tasc will be:
  * Simple creation of a scenario or a situation with sequential flow
  * Designing information transfer for user within context
  * Evaluating user performance on a per-step basis or whole
  * Plug-and-play scenario execution based on Tasc script and engine (e.g., Tasc-Unity)
  * Evaluation of scenario itself (quality of scenario in terms of information transfer)

Tasc has been influenced by several concepts such as `GOMS model <https://en.wikipedia.org/wiki/GOMS>`__ and its variations,
`behavior-driven development (BDD) <https://en.wikipedia.org/wiki/Behavior-driven_development>`__,
`Human processor model (MHP) <https://en.wikipedia.org/wiki/Human_processor_model>`__,
`promise <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise>`__,
`React Hooks <https://reactjs.org/docs/hooks-overview.html>`__,
and `Event-Condition-Action rule model (ECA) <https://en.wikipedia.org/wiki/Event_condition_action>`__.

Related GitHub repositories are:
  * documentation
    * Tasc documentation: (https://github.com/JinkiJung/Tasc)
  * editor
    * Tasc to-do list: (https://github.com/JinkiJung/tasc-todo)
    * Tasc web-editor: (https://github.com/JinkiJung/Tasc-editor)
  * engine
    * Tasc-Unity engine: (https://github.com/JinkiJung/Tasc-Unity)
  * reference implementations with the engine
    * Maze escape 3D as a reference implementation based on Tasc-Unity: (https://github.com/VirtualityForSafety/MazeEscape3D)
    * Stretching exercise 3D as a reference implementation based on Tasc-Unity: (https://github.com/VirtualityForSafety/StretchingExercise3D)
    * Crane manipulation 3D as a reference implementation based on Tasc-Unity: (https://github.com/VirtualityForSafety/CraneManipulation3D)


Current maintainer: `Jinki Jung <https://jinkijung.github.io/>`__

Contents
^^^^^^^^
.. toctree::
   :maxdepth: 3

   gettingStarted
   basicConcept
   terminology
   background
   license
   help



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
