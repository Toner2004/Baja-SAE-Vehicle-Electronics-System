# SRB-25 Vehicle Electronics & Data Acquisition System

Electrical system redesign, wiring harness development, sensor integration, telemetry implementation, and data acquisition support for the Spartan Racing Baja SAE vehicle.

---

## Overview

As Electronics Lead for Spartan Racing Baja, I led the development of the SRB-25 vehicle electronics system. The project focused on improving reliability, documentation, manufacturability, and data acquisition capabilities for a vehicle designed to operate in harsh off-road environments.

The work included:

- Vehicle electrical architecture
- Wiring harness design and routing
- Sensor integration
- Data acquisition support
- Power distribution improvements
- Electrical documentation
- Vehicle testing and validation
- Future telemetry and controller system planning

---

## My Role

### Electronics Lead – Spartan Racing Baja (SRB25)

Responsibilities included:

- Leading vehicle electronics development
- Cross-functional integration with chassis, suspension, and powertrain teams
- Wiring harness architecture and routing
- CAD modeling and packaging
- Sensor integration
- Data acquisition support
- Design reviews
- Bill of materials development
- Electrical documentation
- Future telemetry and controller planning

---

## Project Highlights

### Vehicle Electrical Architecture

Developed a structured electrical architecture to improve reliability, serviceability, and future scalability.

Improvements included:

- Centralized electrical hub
- Fuse block implementation
- Serviceable connector interfaces
- Improved documentation
- Better sensor integration

---

### Wiring Harness Design

The SRB-25 harness was redesigned to improve durability and serviceability while operating in a harsh off-road environment.

#### Right Side Harness

- Brake light circuit
- Differential switch circuit
- Kill switch circuit
- Battery power routing

#### Left Side Harness

- Wheel speed sensors
- Brake pressure sensors
- Suspension travel sensors
- CVT temperature sensor
- Engine RPM sensor
- Camera system

Harness routing was developed using SolidWorks and validated against real vehicle geometry.

---

## CAD-Based Harness Planning

The harness routing model was used to:

- Determine wire lengths
- Support voltage-drop analysis
- Improve serviceability
- Avoid debris and driver contact points
- Guide final vehicle installation

Approximate total wiring:

- ~108 ft of wire
- Power and data harnesses combined

---

## Power Distribution

A centralized electrical hub was introduced to replace scattered inline fuse implementations.

### Features

- Fuse block integration
- Deutsch connector interface
- Simplified troubleshooting
- Easier service access
- Improved reliability

Example circuits:

| Circuit | Fuse |
|----------|--------|
| Evo5 Data Logger | 2 A |
| RPM Sensor | 1 A |
| Polaris Differential | 1 A |
| Brake Light | 1 A |

---

## Sensor Integration

Integrated sensors include:

- 3 Wheel Speed Sensors
- 2 Brake Pressure Sensors
- 4 Suspension Travel Sensors
- CVT Temperature Sensor
- Engine RPM Sensor

These sensors support vehicle testing, tuning, and performance evaluation.

---

## Data Acquisition

The vehicle electrical system supports data acquisition for performance monitoring and testing.

### Telemetry Inputs

- Wheel speed
- Brake pressure
- Suspension travel
- Engine RPM
- CVT temperature

### Design Goals

- Reliable data collection
- Easy troubleshooting
- Future system expansion
- Validation during testing

---

## Vehicle Testing & Validation

The system was tested on the SRB-25 vehicle to verify:

- Harness integrity
- Sensor functionality
- Data acquisition performance
- Telemetry functionality
- Vehicle integration

Testing included on-vehicle validation during Baja SAE development and testing events.

---

## Advanced Vehicle Instrumentation

The team supported advanced vehicle testing efforts using professional-grade instrumentation.

A Michigan Scientific Wheel Force Transducer (WFT) was loaned for vehicle testing and data collection.

The purpose of the testing effort was to:

- Collect wheel force data
- Improve understanding of suspension behavior
- Support future chassis development
- Correlate wheel loads with onboard sensor data

Detailed analysis is still in progress and has been documented separately.

See:

```text
documentation/
└── WFT_Testing_Event.md
```

---

## Documentation

Engineering documentation generated throughout the project included:

- Wiring diagrams
- Sensor channel assignments
- Connector documentation
- Harness routing plans
- Wire length calculations
- Design reviews
- Power distribution studies
- Data acquisition planning

---

## Future Development

### Custom Data Acquisition System

Future efforts aim to reduce dependence on proprietary systems through development of in-house electronics solutions.

Areas under investigation include:

- Custom DAQ systems
- CAN-based communications
- Embedded controllers
- Telemetry systems
- Vehicle networking

### Power Distribution Unit (PDU)

Planned future work includes:

- Fused outputs
- Current sensing
- CAN communication
- 12 V / 5 V / 3.3 V rails
- STM32-based control
- Vehicle diagnostics

---

## Results

The SRB-25 electronics redesign helped:

- Eliminate major harness failure points
- Improve serviceability
- Improve electrical documentation
- Improve vehicle reliability
- Support future electronics development
- Create a foundation for future telemetry and embedded systems projects

---

## Skills Demonstrated

- Vehicle Electronics
- Wiring Harness Design
- Data Acquisition Systems
- Sensor Integration
- Power Distribution
- Fuse Block Design
- CAD-Based Routing
- Electrical Documentation
- Connector Selection
- Vehicle Testing
- Telemetry Systems
- Systems Engineering
- Technical Leadership
- Cross-Functional Engineering Collaboration

---

## Technologies Used

### Software

- SolidWorks
- Altium Designer
- MATLAB
- Python
- GitHub

### Hardware

- AiM EVO5
- Wheel Speed Sensors
- Brake Pressure Sensors
- Suspension Travel Sensors
- RPM Sensors
- Temperature Sensors
- Deutsch Connectors

---

## Repository Structure

```text
SRB25-Vehicle-Electronics-System/
│
├── README.md
│
├── images/
│
├── documentation/
│   ├── WFT_Testing_Event.md
│   ├── Wiring_Harness_Overview.md
│   └── Sensor_Channel_Layout.md
│
├── diagrams/
│
├── calculations/
│
└── cad/
```

---

## Author

Anthony Garcia

Electrical Engineering | Vehicle Electronics | Data Acquisition | Embedded Systems | RF Systems
