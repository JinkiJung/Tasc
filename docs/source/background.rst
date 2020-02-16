Background
==========
Jinki Jung and Hyeopwoo Lee, as a research team, had conducted several series of user experiments on Virtual Reality (VR) and Augmented Reality (AR) based training (virtual training for short).
While repeating similar procedure of developing virtual training, they found out that the core value of the program is transferring the information that should be transferred to a trainee precisely
whereas the implementation of it from a training script is very tough and even risky process when it does not fit to the trainer's expectation.

Field problem
^^^^^^^^^^^^^
During their research, they had several chances of experiencing what happens in the implementation of virtual training in the industry.
At that moment high cost of implementation was expected due to the risk of misalignment of implementation with client's needs, which is a B2B-common problem.
But when there are misalignments on procedure, even worse, the implementation should be start from scratch which increases a significant amount of risks.
They though about an ideal solution that provides common understanding of the procedure and even contributes its implementation.

What matter is procedure
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Even though the visual effects are crucial part of building immersion of virtual training, the procedure within the trainee's experience from it is significantly important as it used as a tool.
Hyeopwoo initially proposed the idea of Pairwise Authoring that organize the procedure with the pairing components of Action and Target, assuming for single user.
The authoring scheme was extended to a triple set of components, i.e., Condition, Terminus, and Action, which was partially presented at the paper 'Annotation vs. Virtual Tutor: Comparative Analysis on the Effectiveness of Visual Instructions in Immersive Virtual Reality'.
As the paper aimed to evaluate user's performance at three different contexts, they confronted the difficulties in the implementation of virtual training and evaluation thereof.
After finalizing the submission, Jinki decided to extend this authoring scheme to be more generic and publish it as open-source.

Procedure description
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The scenario authoring should be simple, informative, but linked to the implementation.
They found out there is no perfect solution to this requirement.
With Hyeopwoo's advice, Jinki developed Tasc-Unity and its reference implementations and extended it to more generic procedure description inspired by Behavior-Driven Development.
Now the objective of Tasc is to be able to represent all kind of procedures and ingest it as executable.
