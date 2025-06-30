# Contact-Free Pedestrian Friendly Traffic Signal using Arduino Uno simulated using Proteus

## About
A smart traffic light system built with Arduino Uno that enables contact-free pedestrian crossing using an ultrasonic sensor, enhancing safety during COVID-19 and improving accessibility.


## Introduction
We all are accustomed to seeing traffic signals, especially in crowded cities. From childhood we have been taught that red means stop, yellow means get ready, and green means go. Traffic lights play an integral role in controlling, directing, and maintaining order amidst the chaos of traffic.

Many modern traffic signals now include a pedestrian button to indicate when someone wants to cross, and some also use audible signals to assist visually impaired pedestrians. This project aims to go a step further by building a **pedestrian-friendly, contact-free traffic signal using Arduino Uno**, reducing the need for physical contact — especially important during the COVID-19 pandemic.

---

## Objective
To build a traffic signal using an Arduino Uno that allows pedestrians to safely signal their intent to cross **without physical contact**, thus improving hygiene and accessibility.

---

## Components
| Component                  | Description                                        |
|-----------------------------|---------------------------------------------------|
| Arduino Uno                 | Microcontroller to control the system logic       |
| 9V Battery                  | Power supply connected to Arduino power jack      |
| LEDs (Red, Yellow, Green)   | Indicate traffic light states                     |
| Resistors (3 x 1200Ω)        | Limit current to LEDs                             |
| Ultrasonic Sensor           | Detects hand wave to trigger pedestrian signal    |
| Buzzer + 100Ω Resistor      | Audible alert for visually challenged pedestrians |
| Jumper Cables               | For connecting all components on breadboard       |

---

## Methodology

### Circuit Design
- **LED Connections:**  
  - Red LED → Pin 3 (via 1200Ω resistor)  
  - Yellow LED → Pin 4 (via 1200Ω resistor)  
  - Green LED → Pin 5 (via 1200Ω resistor)

- **Ultrasonic Sensor:**  
  - Echo → Pin 6  
  - Trigger → Pin 7  
  - VCC → 5V  
  - GND → GND

- **Buzzer:**  
  - Connected via 100Ω resistor to Pin 9 and GND.

![image](https://github.com/user-attachments/assets/8beb4d4f-92a9-4499-9000-3fe012cf7aae)

---

## How It Works
- The traffic light cycles through red, yellow, and green states, controlled by the Arduino Uno.
- The ultrasonic sensor continuously monitors for nearby motion (such as a hand wave). 
- When it detects a pedestrian request:
  - It accelerates the sequence to turn the green pedestrian signal on.
  - The buzzer sounds to indicate it is safe to cross.
- The system then resumes its normal cycle.
- Video demonstration of the same is availble in the repo
