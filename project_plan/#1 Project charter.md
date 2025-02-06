# Line Following and Color-Detecting Robot Car 

## Project Description

Our Line Following and Color-Detecting Robot Car is an autonomous vehicle powered by Raspberry Pi that follows a colored line and changes direction based on the color of the surface beneath it. Equipped with infrared and color sensors, it can stop, turn, or perform actions based on detected colors. This project demonstrates real-time sensor integration and motor control for practical applications in automation and robotics.

**Purpose of the Project**

Autonomous robots that can follow lines and detect colors have significant applications in many industries, offering enhanced efficiency and accuracy. In manufacturing, logistics, and warehousing, these robots can streamline operations by autonomously transporting materials along predefined paths while adjusting to different routes based on color-coded signals. This technology reduces the need for human intervention, leading to faster processing times and minimizing human error.

## Objectives of the Project

Our main goals are:

- Create and build a robotic car capable of following a line using infrared or color sensors, while also detecting various surface colors to adjust its movement as needed.
- Instruct the robot to alter its direction or execute particular tasks depending on the identified color.
- Guarantee smooth, stable, and uninterrupted motion along the path with quick responses to color detection.

### SMART Success Criteria

To ensure the project’s success, we will measure progress against the following SMART criteria:

1. **Color Detection Accuracy**: The robot must accurately distinguish between at least three colors (red, green, blue) on the floor with a minimum 95% detection accuracy under standard lighting conditions, while also observing the background, to differentiate between possibly colorful floor and colored line.
2. **Response Time**: The system must respond to detected color changes within 500 milliseconds to ensure smooth navigation.
3. **Battery Life**: The robot should operate continuously for at least 30 minutes on a single charge while performing all required functions, including movement and color detection.
4. **Completion Time**: The entire project must be completed within given time, including design, testing, and integration phases, to meet the project timeline.

## Constraints of the Project

- The color detection system must accurately distinguish between at least three colors (e.g., red, blue, green) on various surfaces under different lighting conditions.
- The robot will only operate on simple, smooth surfaces (out-of-scope: handling off-road or uneven terrain).
- The robot will be able to distinguish between a line, and a background, even if the floor consists of multiple colors.
- The robot should be able to operate at least half an hour without any charging needed.

## Directions Concerning the Solution

To achieve these goals, we will approach the project in phases that address both hardware and software aspects. Each phase will incorporate testing and adjustments to ensure robust integration and functionality. The main phases include:

1. **Hardware Assembly and Sensor Integration**: Selecting and mounting sensors (both infrared and color) to enable the robot to follow a line and detect surface colors effectively.
2. **Software Development and Calibration**: Writing and testing code for line-following and color-detection algorithms, followed by fine-tuning for responsive movement.
3. **Performance Optimization**: Using feedback control (e.g., PID control) to ensure smooth movement along paths and reliable color-based responses.
4. **System Testing and Refinement**: Conducting extensive testing on different surfaces and lighting to refine the accuracy and stability of the robot’s responses.

These phases will be managed iteratively to allow adjustments based on testing results and stakeholder feedback, maintaining a focus on real-time response and operational efficiency.

## Main Stakeholders and Responsibilities

1. **Team Member 1: [Maciej]**  
   **Role**: Hardware Engineer  
   - Responsible for selecting, assembling, and wiring the robot's physical components, including motors, wheels, chassis, and sensors for both line-following and color detection.
   - Ensure compatibility between sensors, microcontroller, and the motor control system.

2. **Team Member 2: [Matio]**  
   **Role**: Software Engineer and Systems Integration  
   - Responsible for programming the robot’s control system.
   - Write and optimize code for both line-following and color detection functionalities.
   - Coordinate the integration of hardware and software components.
   - Test and debug software components, ensuring the robot can follow the line and respond to color changes as required.

3. **Team Member 3: [Bartosz]**  
   **Role**: Testing Engineer  
   
   - Develop test cases and track performance metrics for both line-following and color detection.
   - Fine-tune the system to ensure the robot achieves its performance targets, including color detection accuracy and smooth navigation.
   - Test hardware durability and sensor accuracy.

## Risks Identified Early On

1. **Risk: Sensor Interference**  
   **Description**: Environmental factors, such as inconsistent lighting, could affect the color sensor’s accuracy, leading to incorrect color detection and potentially causing the robot to follow an incorrect path.
   **Mitigation Plan**:
      - **Calibration**: Perform sensor calibration in varied lighting conditions (e.g., dim, fluorescent, natural sunlight).
      - **Lighting Shields**: Use shielding around the sensors to minimize external light interference.
      - **Fallback Detection**: Implement additional logic in software to double-check colors if rapid changes are detected.

2. **Risk: Hardware Limitations (Battery Life and Motor Durability)**  
   **Description**: Extended operation may lead to quicker battery depletion or motor overheating, potentially affecting performance.
   **Mitigation Plan**:
      - **Power Management**: Optimize power usage in code (e.g., turning off sensors or reducing motor speed when idle).
      - **Cooling Intervals**: Add programmed breaks to avoid continuous motor usage, if necessary.
      - **Spare Components**: Keep backup motors and batteries available to swap in quickly if necessary.

## Target Project Benefits

This project aims to produce a functional, autonomous robot that can:

- **Adapt to Dynamic Environments**: By detecting and responding to different colors, the robot can navigate through varied paths, demonstrating real-time adaptability.
- **Provide a Model for Automation Applications**: The line-following and color-detecting functionalities offer a foundational approach applicable in sorting, transport, and logistics systems.
- **Enhance Learning in Robotics**: This project serves as an educational platform for learning about sensor integration, motor control, and real-time processing in robotics.
