# CPSC-359-Assignment-1-Combibot-a-sumobot-strategy-in-combinatinal-logic-solution

Download Here: [CPSC 359 Assignment 1: Combibot: a sumobot strategy in combinatinal logic solution](https://jarviscodinghub.com/assignment/assignment-1-combibot-a-sumobot-strategy-in-combinatinal-logic-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Background
“Robot-sumo is a sport in which two robots attempt to push each other out of a circle (in a similar fashion to the sport
of sumo). The robots used in this competition are called sumobots.” (https://en.wikipedia.org/wiki/
Robot-sumo) In this assignment, you will design a combinational logic circuit to implement a simple strategy for a
hypothetical sumobot.
Combibot
Figure 1 describes the basic operation of the combibot and the sumo arena in which it competes.
Combibot balances on two wheels, controlling its motion with the motors that drive those wheels. It uses differential steering, i.e., steers by turn the wheels in different directions or at different rates. You have two motor controllers,
one for each wheel, and each motor can do only one of three things at any point in time: stop, go forward, or go
in reverse. Table 1 summarizes the binary inputs to the motor controllers. Note that the motor controllers do not
respond continuously to their input – they sample the command input once every second, performing the commanded
behaviour for a full second before getting the next command.
Combibot has four sensors, each of which produces a binary value depending on what it senses. M0 and M1 detect
the edge (or margin) of the arena. M0 looks forward while M1 looks rearward. M0 = M1 = 0 means combibot is
inside the arena, while M0 = 1 or M1 = 1 means the corresponding side of combibot is at the edge of the arena. E0
and E1 detect the opponent sumo (or enemy). E0 looks to the left, and E1 looks to the right. E0 = 0 or E1 = 0 means
no opponent detected, while E0 = 1 or E1 = 1 means an opponent is detected on the corresponding side of combibot.
What you need to do
To design the circuit and complete the assignment, you need to do the following.
1. Identify all the inputs and outputs for your circuit. This step is fairly obvious, but it is a good habbit to write
these down anyway.
L1(R1) L0(R0) action
0 0 stop
0 1 forward
1 0 reverse
1 1 not allowed
Table 1: Motor control commands. L1/L0 (left wheel) and R1/R0 (right wheel) are binary inputs. The controllers
sample their input to get a commandevery second. They perform the last command received for a full second until
they get the next command.
forward
balances on
two wheels
front
sensor
side
sensor
M0
M1
E0 E1
left
motor right
motor
forward motion
(a) (b)
combat area
(approx 1m diameter)
combat perimeter
(color change for photo sensor)
(c)
Figure 1: Combibot and the sumo combat arena: (a) a sketch of a combibot, (b) a top view showing sensor and motor
layout, and (c) the arena.
2. Use the combibot strategy sheet provided to develop your strategy for combinational control of combibot. You
are free to create your own strategy, but it must be reasonable. I.e., your strategy should look like it could
possibly win a Robo-sumo competition against a weak opponent. Strategies that the marker deems overly
simple (in order to trivialize the circuit design) will receive low grades.
3. Design the combinational circuits to implement your strategy.
4. Implement your design in Logisim using the provided template.
Deliverables
Turn in the following items for evaluation.
1. Documents (and code) to show the steps in your analysis and design for items 1, 2 and 3 above. You can scan
your combibot strategy sheet, or annotate the pdf electronically. You should also include truth tables, Karnaugh
maps, and functions in minimized disjunctive normal form (OR of ANDs).
2. All files for your Logisim implementation of your design (probably just one).
Evaluation
1 Identification of input/output/state variables. 2pts
2 Karnaugh maps for each output. 6pts
3 Design of combinational logic for each output. 5pts
4 Logisim implementation – runs correctly. 5pts
5 Logisim implementation – inputs/outputs labelled. 2pts
Total 20pts
There is no team work. Each student should submit their own solution.
Late work
After the deadline and up to 24hrs late: -5pts. After 24hrs and up to 48hrs late: -10pts. Over 48hrs late: -20pts, i.e.,
no assignment will be accepted beyond 48hrs after the deadline.
Plagiarism
Submitted solutions must be your own work, and only your own work.
You may find that the design task for this assignment is similar to other well known circuits. Nevertheless, you
should go through the design process yourself, and submit your own work. If you do borrow from other sources, cite
the source and clearly indicate what you have borrowed, keeping in mind the design must be substantially your own.
If you cite your sources, worst case you may receive a reduced grade for borrowing too much. If you borrow, but do
not cite, that is plagiarism and academic misconduct. Plagiarism carries severe penalties as determined by the Faculty
of Science.
As a guideline, consider the 20-minute rule. Talk with your colleagues and consult other sources (cite them please).
Wait at least 20 minutes, then do your work to be sure that it is your own. Less then 20 minutes usually means that
you are merely copying work from the original source.

