# SRB-25 Vehicle Electronics & Data Acquisition System

Electrical system redesign, wiring harness development, sensor integration, and data acquisition planning for the Spartan Racing Baja SAE vehicle.

---

## Overview

As Electronics Lead for Spartan Racing Baja, I led the development of the SRB-25 vehicle electronics system. This work focused on improving the reliability, serviceability, documentation, and integration of the vehicle electrical architecture for harsh off-road competition environments.

The project included:

- Vehicle electrical system architecture
- Wiring harness redesign
- CAD-based harness routing
- Power distribution improvements
- Sensor wiring and channel planning
- Data acquisition support
- Electrical documentation
- Future controller, telemetry, and power distribution development

---

## Project Background

The previous SRB-24 electrical system had several issues related to packaging, connector reliability, harness protection, sensor placement, and serviceability. The SRB-25 redesign focused on addressing those weaknesses through a more structured electrical architecture and improved documentation.

Key problems identified in the previous system included:

- Data acquisition hardware placed in a poor location
- Limited driver-area clearance
- Old and frayed wiring
- Non-automotive connectors
- Loose connections inside the harness
- Limited water resistance
- Sensor routing and mounting failures
- Poor dashboard placement
- Vulnerable GPS mounting location

---

## My Role

**Electronics Lead – Spartan Racing Baja SRB-25**

My responsibilities included:

- Leading vehicle electronics development
- Coordinating integration with powertrain, suspension, chassis, and competition requirements
- Designing the electrical system for power and data
- Developing wiring harness routing in CAD
- Creating bills of materials
- Supporting data collection sensor systems
- Supporting controller and telemetry system planning
- Training and coordinating new electronics members

---

## System Architecture

The SRB-25 electronics system was organized around several major subsystems:

- Electrical hub
- Power distribution
- Wiring harness
- Sensor wiring
- Data acquisition
- Controller and telemetry development
- Documentation databases

---

## CAD-Based Wiring Harness Routing

The SRB-25 harness was routed using CAD models to better reflect real vehicle geometry and real harness lengths.

The routing model was used to:

- Plan harness paths along chassis members
- Avoid driver egress areas
- Reduce exposure to road debris
- Estimate real wire lengths
- Support voltage drop calculations
- Guide physical harness installation

<p align="center">
  images/srb25_harness_routing_model.png
</p>

The final harness model included approximately 108 ft of combined power and data wiring.

---

## Wire Length Planning

Wire lengths were estimated from the CAD routing model and translated into real vehicle harness lengths.

### Right Side Harness

Included:

- Brake light wiring
- Differential power
- Kill switch wiring
- Battery power routing

Example planned lengths:

- Brake light power to middle hydraulic switch: 62 in
- Brake light power to front hydraulic switch: 125 in
- Differential power line: 142 in
- Differential switch line: 115 in
- Kill switch splice to driver: 96 in
- Electrical hub to battery: 71 in

<p align="center">
  images/right_side_wire_lengths.png
</p>

### Left Side Harness

Included:

- Brake pressure sensors
- Linear travel sensors
- Wheel speed sensors
- Driver dash wiring
- Camera wiring
- CVT temperature sensor
- RPM sensor

<p align="center">
  images/left_side_wire_lengths.png
</p>

---

## Electrical Hub

The SRB-25 vehicle introduced a centralized electrical hub instead of relying on inline fuses throughout the harness. This made the system easier to inspect, troubleshoot, and service.

The electrical hub included:

- Fuse block
- Power distribution wiring
- Deutsch connector interface
- Improved fault isolation
- Cleaner electrical packaging

<p align="center">
  images/srb25_electrical_hub.png
</p>

### Example Fuse Assignments

| Circuit | Fuse |
|--------|------|
| Evo5 Data Logger | 2 A |
| RPM Sensor | 1 A |
| Front Polaris Differential | 1 A |
| Brake Light | 1 A |

---

## Vehicle Wiring Documentation

A vehicle wiring diagram was created to document both data and power connections. This documentation served as the foundation for future electronics troubleshooting and team knowledge transfer.

Documented systems included:

- Engine kill switch
- Brake lights
- 4WD switch
- Analog channels for data acquisition
- Extra appliances such as cameras and screens
- Power lines

<p align="center">
  images/vehicle_wiring_diagram.png
</p>

---

## Sensor Wiring and Data Acquisition

The sensor wiring system was documented to support custom data lines and data acquisition channel planning.

Integrated sensor channels included:

- 3 wheel speed sensors
- 2 brake pressure sensors
- 4 linear travel sensors
- CVT temperature sensor
- Engine RPM signal

<p align="center">
  images/sensor_wiring_diagram.png
</p>

---

## Analog Channels and CAN Bus

Analog channel profiles were configured based on sensor characteristics and useful data update rates. The goal was to capture meaningful vehicle data while keeping the data acquisition system efficient.

Examples of considerations:

- Brake pressure did not require extremely high update rates
- Suspension components could operate at lower update rates
- RPM data required higher update rates for meaningful analysis
- Sensor profiles were adjusted as testing continued

<p align="center">
  images/analog_channels_can_bus.png
</p>

---

## Data Acquisition Direction

Future work began moving away from expensive proprietary data acquisition hardware toward lower-cost custom platforms.

Motivations included:

- Reducing system cost
- Reducing dependence on proprietary hardware
- Improving repairability
- Supporting future custom telemetry and controller systems

<p align="center">
  <imges/future_daq_work.png
</p>

---

## Future Power Distribution Unit

A future SRB-26 power distribution unit was proposed as the next step toward a custom vehicle electronics platform.

The concept included:

- Low-voltage power board
- Fused outputs
- Current sensing
- 12 V, 5 V, and 3.3 V buses
- CAN communication
- STM32-based control
- Shunt circuits
- Regulators
- Gate drivers
- Trace width calculations

<p align="center">
  images/future_pdu_concept.png
</p>

---

## Documentation and Knowledge Transfer

A major goal of the electronics effort was creating documentation that could survive beyond one design cycle. The team used structured databases and engineering tools to organize design files, drawings, revisions, and build information.

Tools and documentation systems included:

- SolidWorks PDM
- Altium
- GitHub
- Google Drive / Excel databases

<p align="center">
  images/electronics_database.png
</p>

---

## Results

The SRB-25 electronics redesign helped:

- Eliminate major harness failure points
- Improve reliability in harsh environments
- Introduce a structured electrical architecture
- Improve documentation for future team members
- Reduce reliance on expensive proprietary systems

---

## Skills Demonstrated

- Vehicle electrical system design
- Wiring harness design
- CAD-based harness routing
- Power distribution
- Fuse block planning
- Sensor integration
- Data acquisition systems
- CAN bus concepts
- Electrical documentation
- System integration
- Design review communication
- Technical leadership
- Cross-functional engineering coordination

---

## Suggested Repository Structure

```text
SRB25-Vehicle-Electronics-System/
│
├── README.md
│
├── images/
│   ├── srb25_harness_routing_model.png
│   ├── right_side_wire_lengths.png
│   ├── left_side_wire_lengths.png
│   ├── srb25_electrical_hub.png
│   ├── vehicle_wiring_diagram.png
│   ├── sensor_wiring_diagram.png
│   ├── analog_channels_can_bus.png
│   ├── future_daq_work.png
│   ├── future_pdu_concept.png
│   └── electronics_database.png
│
├── documentation/
│   ├── sanitized_design_summary.md
│   ├── harness_notes.md
│   └── sensor_channel_notes.md
│
├── diagrams/
│   ├── power_distribution_overview.png
│   ├── harness_block_diagram.png
│   └── sensor_channel_overview.png
│
└── calculations/
    ├── wire_length_summary.xlsx
    ├── voltage_drop_notes.md
    └── fuse_assignment_table.xlsx
```

---

## Author

Anthony Garcia  
Electrical Engineering | Vehicle Electronics | Wiring Harness Design | Data Acquisition | RF & Embedded Systems
