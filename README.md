Traffic Light System for 4-Way Intersection
Overview
This project simulates a 4-way traffic light system designed to manage vehicle flow at an intersection with entries from the North, East, South, and West directions. The system cycles through states to control the Red, Yellow, and Green lights for each direction, ensuring smooth and safe traffic management.

Project Structure
State Diagram: Illustrates the traffic light states (S1-S8) and their transitions, with specific timings for each light color (Green and Yellow).
Sequence Diagram: Displays the event sequence for each direction, showing the light color changes for North, East, South, and West entries.
Key Features
Traffic Light Cycles: The system uses a cycle with 8 states (S1-S8), each representing an active traffic light phase.
Emergency State: An override state enables all lights to be controlled by an emergency condition, allowing traffic control adjustments as needed.
Timing and Transitions: Each state includes specific durations for Green and Yellow lights.
State and Sequence Details
State Diagram
The state diagram demonstrates each phase (S1-S8) and the transitions between them. Each state controls a specific direction with the following timing:

Green Light: 30 seconds
Yellow Light: 5 seconds The diagram includes arrows indicating state transitions, showing the system's flow as it cycles through each direction.
Sequence Diagram
The sequence diagram outlines the flow of events, with each lane (North, East, South, and West) showing the color change sequence over time:

Green Light Activation - Allows traffic in the active direction.
Yellow Light Activation - Signals the end of the Green phase.
Red Light Activation - Stops traffic while other directions activate.
Usage Instructions
Cycle Management: The system automatically transitions through states S1 to S8, controlling the active light colors for each direction.
Emergency Override: In the event of an emergency, the system enters the Emergency state, pausing the normal cycle to prioritize traffic management as needed.
Example Timings
State	Active Light (Direction)	Green Duration	Yellow Duration
S1	North	30s	5s
S2	East	30s	5s
S3	South	30s	5s
S4	West	30s	5s
Future Improvements
Dynamic Timing: Allowing configurable Green and Yellow light durations based on real-time traffic conditions.
Pedestrian Signals: Adding pedestrian signal management to increase safety and control.
Requirements
This project was designed with basic diagrams; tools like draw.io can be used to visualize and modify the state and sequence diagrams.
