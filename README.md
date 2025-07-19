# Overall Description 
This project simulates a fully automated assembly and packaging line using Factory I/O and the Control I/O interface, without the use of an external PLC. The system is composed of two synchronized pick-and-place machines that assemble two separate components into a single final product. Once assembled, the product is transferred onto a conveyor belt and delivered to the packaging area.

The line features sensors, electrical push buttons, counter displays, and actuators arranged to replicate a realistic industrial setting. The project allows the user to define the number of combined parts per packaging box, demonstrating parameterized control logic. 

-The control logic is fully implemented using the Control I/O interface in Factory I/O. The program includes:
-Set/Reset latching logic
-Counters for part tracking and box count
-On-delay and off-delay timers
-Rising edge and falling edge triggers for event detection
-Manual/automatic operation mode
-Stop/reset functionality for system reliability

The system is designed to be flexible and configurable. The number of assembled parts per packaging box and the number of boxes per cycle can be customized through internal counter settings. For example:
Scenario 1: The system is set to place 1 assembled part per box. This sequence is repeated to produce 2 packed boxes, demonstrating basic functionality as shown in (Video: Part1).
Scenario 2: The system is reconfigured to pack 2 assembled parts per box, and the sequence continues until 5 boxes are completed, showcasing more advanced batching and cumulative logic.

The logic ensures precise coordination between the pick-and-place units, conveyors, and packaging mechanism, while maintaining flexibility in batch size. This setup reflects key concepts in industrial automation, such as discrete manufacturing, sequencing, and basic recipe control.

# Description of Video Part 1 
This video provides an overview of the automated assembly line, showcasing the layout of sensors, counter displays, machines, and conveyors. It is followed by a presentation of the control logic implemented using the Control I/O interface in Factory I/O. The video first introduces the system's operational flow, then transitions to the Control I/O panel to explain the program structure, I/O mapping, and the sequencing logic. The control program utilizes key automation functions such as Set/Reset latches, counters, on-delay and off-delay timers, as well as rising and falling edge triggers all coordinated to manage the assembly and batch packaging process.

# Description of Video Part 2 
Part 2 of the video demonstrates the system in operation with the number of combined parts per packing box set to 1. The process is then repeated, resulting in a total of two packed boxes by the end of the sequence.
