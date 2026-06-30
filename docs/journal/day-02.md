# Day 2 – Requirements Engineering

Date: 2026-06-30

## Objectives

- Define the project vision.
- Choose a realistic system scenario.
- Start Software Requirements Specification (SRS).
- Introduce UML and PlantUML.

---

## Accomplishments

### Project Charter

Created the initial Project Charter and defined:

- Mission
- Goals
- Success Criteria
- Constraints
- Guiding Principles

---

### System Scenario

Selected an Industrial AGV (Autonomous Guided Vehicle) as the target system.

The robot will support:

- Manual Mode
- Autonomous Mode
- Emergency Mode

---

### Hardware Components

#### Sensors

- Temperature
- Humidity
- GPS
- IMU
- Wheel Encoders
- Battery Monitor
- Ultrasonic Distance Sensor
- Camera

#### Actuators

- Drive Motors
- Camera Gimbal

---

### Communication Interfaces

- Serial
- TCP
- MQTT
- RabbitMQ (future)

---

### Requirements Engineering

Started the first version of:

```text
docs/srs/srs-v1.0.md
```

Defined:

- Actors
- Functional Requirements
- Non-Functional Requirements
- System Scope

---

### Diagrams

Installed PlantUML.

Created the first UML diagram:

```text
docs/diagrams/use-case-diagram.puml
```

---

## Key Decisions

### System Type

The project will simulate an industrial AGV instead of a simple educational robot.

### Architecture

The project will later adopt:

- Clean Architecture
- MVVM
- Domain-Driven Design (DDD)

---

## Lessons Learned

- Requirements should be written before implementation.
- Use Cases drive architecture.
- Domain modeling starts from understanding the business problem.
- Diagrams should be version-controlled like source code.

---

## Challenges

The system scope is intentionally large and will require incremental development.

---

## Next Steps

- Complete Use Cases.
- Create Domain Model.
- Create Architecture Decision Records (ADR).
- Design the initial software architecture.