# Robotics

  This project represents a successful implementation of a robotic navigation system that leverages line tracking and obstacle avoidance to autonomously guide the Finch Robot along a designated path while ensuring it can detect and navigate around obstacles. The primary objective was to create a robot that could accurately follow a line, intelligently avoid obstacles in its path, and return to its original trajectory seamlessly.
 The main user requirement for this project was to design a navigation system where the robot could:
  - Follow a defined path using its line sensors
  - Detect and navigate around obstacles using its ultrasonic sensor
  - Indicate status updates via LED signals
  - Allow for manual stopping via keyboard input

  To achieve this, the system was built using Java, leveraging object-oriented programming principles to ensure modularity and maintainability. The program consists of several key components:

  Line Tracking: The Finch uses two infrared sensors to detect and follow a black line, making small adjustments based on sensor readings to stay on track.
  Obstacle Avoidance: If an obstacle is detected within 20 cm, the robot evaluates the best direction to navigate around it. After successfully avoiding the obstacle, it resumes path following automatically.
  LED Status Indicators:
  - Green Light: Normal path-following operation.
  - Red Light: Robot lost the line and is searching for the path.
  - Yellow Light: Robot is actively avoiding an obstacle.
  
  The development process for this project followed a structured and iterative approach. Since robotics requires constant testing in real-world conditions, the project was developed using incremental improvements, ensuring each functionality worked independently before integrating it into the larger system.
  - Breaking Down the Problem:
Instead of designing the entire system at once, I broke the problem into smaller, testable units. I first developed basic movement functions, then implemented line tracking, followed by obstacle detection, and finally integrated everything into a cohesive system.

  - Testing & Debugging:
Unlike traditional software development where debugging is limited to console logs, debugging a physical robot required real-world testing. This involved observing the robot’s behavior, making code adjustments, and re-running tests multiple times to ensure proper functionality.

  - Overcoming Key Challenges:
The most challenging aspect of the project was fine-tuning the line-following behavior to ensure smooth navigation. Initially, the robot exhibited jerky movements, frequently losing track of the line or making unnecessary corrections. This was improved by adjusting the threshold values of the IR sensors and fine-tuning motor speeds for smoother directional adjustments.

Additionally, obstacle avoidance required precise turning and movement adjustments to ensure the robot could successfully maneuver around objects without getting stuck or veering too far from the original path.

  To ensure reliability, I conducted several real-world tests:
  Line Following Tests:

  Verified that the robot could accurately follow a black line on different surfaces (tile, wood, carpet).
  Adjusted sensor thresholds to ensure optimal line detection.
  Obstacle Avoidance Tests:

  Placed obstacles at various distances and angles along the robot’s path.
  Adjusted the turning algorithm to ensure the robot efficiently avoided obstacles and returned to the path.
  Verified that LED indicators correctly reflected the robot’s status.
  After extensive testing, the robot successfully navigates its path, avoids obstacles dynamically, and recovers lost paths efficiently.

While this version of the project successfully meets the outlined requirements, there are several enhancements that could further improve performance:
  - Implementing PID Control: A more advanced approach to line tracking, using a Proportional-Integral-Derivative (PID) controller, could make the robot’s movements even smoother and more precise.
  - Adding Real-Time Data Logging: Storing sensor data for analyzing movement patterns could help optimize performance.
  - Enhancing Obstacle Avoidance: Using AI-based decision-making to choose the best path rather than just checking left and right.
  - Integrating Wireless Commands: Allowing remote control via a mobile app for added functionality.

  This project was a significant step forward in my development as a robotics programmer. It reinforced object-oriented programming principles, strengthened my debugging and testing skills, and provided valuable experience in real-world robotic control systems. Despite the challenges, the process of building, refining, and successfully deploying this autonomous navigation system was incredibly rewarding.

  This experience has given me greater confidence in my ability to design, implement, and troubleshoot complex robotic systems, and I look forward to building even more advanced robotics applications in the future. 
