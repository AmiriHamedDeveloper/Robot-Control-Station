# Software Requirements Specification (SRS)

## Project

Robot Control Station (RCS)

Version: 1.0 (Draft)

---

# 1. Introduction

## 1.1 Purpose

The purpose of this document is to define the functional and non-functional requirements of the Robot Control Station (RCS) system.

The application provides a desktop control station for monitoring and controlling an Industrial Autonomous Guided Vehicle (AGV) equipped with various sensors, actuators, and communication interfaces.

---

## 1.2 Scope

The system shall provide:

* Robot monitoring and telemetry visualization.
* Manual and autonomous operation modes.
* Communication with the robot through multiple protocols.
* Sensor monitoring.
* Camera streaming.
* Session recording and replay.
* Alarm and emergency management.
* Extensible support for future devices and modules.

---

## 1.3 Definitions and Acronyms

| Term      | Description                          |
| --------- | ------------------------------------ |
| AGV       | Autonomous Guided Vehicle            |
| RCS       | Robot Control Station                |
| Telemetry | Runtime data received from the robot |
| Operator  | Human user of the application        |
| Mission   | A set of tasks assigned to the robot |

---

# 2. Overall Description

## 2.1 Product Perspective

The system is a desktop application that communicates with an Industrial AGV and provides:

* Monitoring
* Control
* Configuration
* Diagnostics
* Data Recording

---

## 2.2 Product Functions

The system shall:

* Connect to the robot.
* Display telemetry.
* Control robot movement.
* Switch operation modes.
* Display camera streams.
* Record sessions.
* Replay recorded sessions.
* Configure communication channels.
* Manage alarms and emergency situations.

---

## 2.3 User Classes

### Operator

Controls and monitors the robot.

### Administrator

Configures the system and communication parameters.

### Maintenance Engineer

Performs diagnostics and troubleshooting.

---

## 2.4 Operating Environment

* Linux (Primary Platform)
* Windows (Secondary Platform)

Technology Stack:

* C++20
* Qt 6
* QML
* CMake

---

# 3. External Interfaces

## 3.1 Serial Communication

Used for:

* Motor controller
* Embedded controller
* Diagnostic devices

---

## 3.2 TCP Communication

Used for:

* Remote monitoring
* Telemetry
* Command exchange

---

## 3.3 MQTT Communication

Used for:

* Telemetry publishing
* Remote commands
* Cloud integration

---

## 3.4 Camera Interface

Used for:

* Live video streaming
* Snapshot capture

---

# 4. Functional Requirements

## FR-001

The system shall connect to the robot.

---

## FR-002

The system shall disconnect from the robot.

---

## FR-003

The system shall display robot telemetry.

---

## FR-004

The system shall display sensor information.

---

## FR-005

The system shall allow manual movement control.

---

## FR-006

The system shall switch between Manual and Autonomous modes.

---

## FR-007

The system shall display live camera streams.

---

## FR-008

The system shall record telemetry sessions.

---

## FR-009

The system shall replay recorded sessions.

---

## FR-010

The system shall configure communication interfaces.

---

## FR-011

The system shall display alarms and warnings.

---

## FR-012

The system shall stop the robot during emergency situations.

---

# 5. Non-Functional Requirements

## NFR-001

The application shall remain responsive during communication and data processing.

---

## NFR-002

The application shall support future extension without significant architectural changes.

---

## NFR-003

The application shall be testable.

---

## NFR-004

The application shall be maintainable.

---

## NFR-005

The application shall support multiple communication protocols.

---

## NFR-006

The application shall support logging and diagnostics.

---

# 6. Assumptions and Constraints

## Assumptions

* A robot simulator may be used before real hardware becomes available.
* Communication interfaces may be unavailable during development.

## Constraints

* Qt/QML shall be used for the user interface.
* C++ shall be used for application development.
* The application shall follow Clean Architecture and MVVM.

---

# 7. Future Enhancements

* RabbitMQ integration
* Plugin architecture
* Multi-robot support
* Mission planning
* Map visualization
* Path planning
* Remote update system
* Web dashboard

