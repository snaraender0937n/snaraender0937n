# Naraender S.

Electrical and electronics engineering student focused on hardware engineering, embedded systems, industrial automation, and software systems.

I design, build, and audit technical projects spanning printed circuit board (PCB) layout, switched-mode power supplies, analog circuits, multi-microcontroller embedded systems, and full-stack software applications. My work emphasizes physical design calculations, firmware safety routines, reproducible build and test environments, and transparent documentation of system constraints.

---

## Areas of Interest

- **Hardware Design & PCB Engineering**: Schematic capture, through-hole and surface-mount (SMD) layout, design rule checking (DRC), electrical rules checking (ERC), single- and double-sided board design, chemical wet etching, and Gerber manufacturing generation.
- **Power Electronics & Analog Circuits**: Switched-mode power topologies (DC-DC buck converters), linear regulator power distribution (+5V, +12V, -12V), operational amplifier signal synthesis (Wien bridge oscillators, comparators, active wave shapers), and component stress audits.
- **Embedded Systems & Robotics**: Bare-metal and RTOS-compatible microcontroller firmware, hardware timers, fast PWM generation, analog-to-digital conversion, sensor interfacing, and multi-protocol motor control with safety watchdogs.
- **Telemetry & Communications**: Synchronized multi-sensor edge data collection, binary struct serialization across mixed processor architectures, RF networking (ESP-NOW, BLE, Wi-Fi SoftAP, cellular LTE Cat-1/GNSS), and industrial messaging protocols (MQTT).
- **Software Systems & Anomaly Analytics**: Full-stack web dashboards, REST APIs, WebSocket streaming pipelines, frequency- and time-domain signal processing (FFT, Crest Factor, Kurtosis), robust non-parametric anomaly detection, and fraud risk scoring.

---

## Technical Skills

- **Programming Languages**: C (C99), C++ (C++17), Python, TypeScript, JavaScript, Embedded C / Arduino C++, HTML5, CSS3.
- **Microcontrollers & Architectures**: ESP32 (Xtensa 32-bit dual-core), ESP32-C3 (RISC-V 32-bit), ESP32-S3, STM32F446RE (ARM Cortex-M4), ATmega328P (AVR), ATtiny85, 74LS TTL / CD4000 CMOS digital logic ICs.
- **Hardware & EDA Tools**: KiCad, SPICE / analog circuit simulation, digital storage oscilloscopes, multimeters, breadboard and chemical wet-etch prototyping.
- **Protocols & Interfaces**: UART, I2C, SPI, ESP-NOW (2.4 GHz RF), Bluetooth Low Energy (BLE / NimBLE), MQTT, WebSockets, HTTP/REST.
- **Sensors & Actuators**: MAX30102 (pulse oximetry / SpO2), MPU6050 (6-axis IMU), DS18B20 (1-Wire temperature), AD8232 (analog ECG AFE), Plantower PMS5003 (particulate matter), HC-SR04 (ultrasonic), SIMCOM SIM7670G (LTE Cat-1 / GNSS), L298N dual H-bridge, relays, and servo motors.
- **Software Frameworks & Libraries**: Node.js, Express, Next.js 14, React 18, Flask, FastAPI, Vite, Socket.IO, Prisma.
- **Databases & Data Stores**: SQLite, PostgreSQL (DDL schema design and relational queries).
- **Development & Verification Tools**: Git, GitHub, pytest, Jest / Vitest, npm, Arduino CLI.

---

## Featured Projects

### Hardware and Embedded Engineering (NaraenderHardware)

#### 1. PCB Design & Manufacturing Engineering
- **Repository**: [pcb-design-manufacturing-engineering](https://github.com/NaraenderHardware/pcb-design-manufacturing-engineering)
- **Description**: Documentation and CAD design files for four hardware case studies covering circuit design, schematic capture, component selection, board layout, and fabrication methods. The projects include a 5V 1.5A through-hole regulated DC power supply, a 3-rail surface-mount linear supply (+5V, +12V, -12V), an ATtiny85 USB Type-A breakout dongle with 3.6V Zener level clamping, and a manual single-sided chemical-etched regulator bench prototype using ferric chloride. Includes Bill of Materials, design calculation audits, Gerber exports, and recorded laboratory multimeter readings.
- **Technologies**: KiCad, PCB Layout, Schematic Capture, Through-Hole & SMD Design, Gerber Generation, LM7805, DPAK Regulators, ATtiny85-20S, Chemical Wet Etching.

#### 2. Power Electronics & Analog Circuit Engineering
- **Repository**: [power-electronics-analog-circuit-engineering](https://github.com/NaraenderHardware/power-electronics-analog-circuit-engineering)
- **Description**: Two hardware engineering case studies analyzing power conversion and analog signal generation. The first is an open-loop 36V to 18V (24W, 50 kHz) DC-DC buck converter powered by an ATmega328P Timer1 fast PWM generator, driving an IRLZ44N power MOSFET through a TLP350 opto-isolated gate driver. The second is a multi-waveform analog function generator producing sine, square, and triangle waves using five uA741 operational amplifiers and a +/-12V linear dual power supply. The repository includes circuit schematics, PCB photographs, automated Python calculation verification scripts, oscilloscope captures, and failure mode audits.
- **Technologies**: ATmega328P, Timer1 Fast PWM, IRLZ44N Power MOSFET, TLP350 Gate Driver, uA741 Operational Amplifiers, Wien Bridge Resonant Tank, Linear Power Regulators, Python, Oscilloscope Characterization.

#### 3. Embedded Control, Automation & Robotics
- **Repository**: [embedded-control-automation-robotics](https://github.com/NaraenderHardware/embedded-control-automation-robotics)
- **Description**: Six embedded control, robotics, and automation case studies accompanied by firmware source code, architectural documentation, and verification suites. Implementations include an STM32F446RE and ESP32 industrial conveyor control system with atomic emergency stop logic, a dual-rail temperature indicator with display debouncing, an autonomous closed-loop plant watering system with pump runaway protection, a 4-bit synchronous TTL/CMOS seven-segment counter, an ESP32 dual-unit BLE RC car with packet-heartbeat watchdog failsafes, and an Arduino ultrasonic radar scanner with PC GUI. Supported by 12 passing Python unit tests and firmware targets compiled via Arduino CLI.
- **Technologies**: STM32F446RE (ARM Cortex-M4), ESP32, Arduino Nano / Uno (ATmega328P), CD4516 CMOS, 74LS TTL Logic, BLE (NimBLE), UART, I2C, Arduino CLI, Python (pytest).

#### 4. VitalEdge: Embedded Telemetry Monitoring System
- **Repository**: [vitaledge-embedded-telemetry-monitoring](https://github.com/NaraenderHardware/vitaledge-embedded-telemetry-monitoring)
- **Description**: An edge-first telemetry prototype collecting synchronized physiological, motion, thermal, environmental, and spatial metrics. Employs a dual-microcontroller architecture: a wearable sensor node (Seeed Studio XIAO ESP32-C3 RISC-V) interfaced with pulse oximetry, analog ECG, 6-axis IMU, digital temperature, and particulate sensors, broadcasting 56-byte packed binary structs via ESP-NOW to an isolated communications gateway (LilyGO ESP32-S3 with SIM7670G LTE/GNSS). Includes a Python/FastAPI ingestion backend, full-duplex WebSocket broadcaster, SQLite historian, and a React monitoring dashboard.
- **Technologies**: ESP32-C3 (RISC-V), ESP32-S3, ESP-NOW RF, MAX30102, MPU6050, DS18B20, AD8232, PMS5003, SIM7670G (LTE Cat-1 / GNSS), Python, FastAPI, WebSockets, React, Vite, SQLite.

---

### Software and Analytics Engineering (NaraenderSoftware)

#### 5. Industrial Fleet Condition Monitoring
- **Repository**: [industrial-fleet-condition-monitoring](https://github.com/NaraenderSoftware/industrial-fleet-condition-monitoring)
- **Description**: An end-to-end industrial telemetry and condition monitoring platform demonstrating real-time vibration analysis, non-parametric anomaly detection, and cross-device regional conflict coordination. Computes time-domain vibration metrics (Peak, RMS, Crest Factor, Kurtosis) and Radix-2 FFT spectral analysis, combined with a rolling dual-window Median and Median Absolute Deviation (MAD) classifier to identify five distinct mechanical and sensor failure modes (spike, drift, flatline, oscillation, sensor swap). The architecture features an Express/TypeScript ingestion server, SQLite and PostgreSQL database schemas, Socket.IO live updates, and a Next.js 14 operator console. Supported by 62 passing automated unit tests across 13 suites.
- **Technologies**: TypeScript, Node.js, Express, Next.js 14, React, Socket.IO, Prisma, SQLite, FFT / Spectral Analysis, MQTT.
- **Verification Status & Documented Limitations**: Evaluated using calibrated synthetic datasets and telemetry generators. Native C/C++ compilation of edge simulators (agent-c and agent-cpp) is unverified in the evaluation environment due to absent host C/C++ build toolchains, although the FFT algorithms and Hann windowing are mathematically verified. Execution of the optional Python ML service (ml-service with Isolation Forest) is unverified on deep Windows directory paths due to operating system MAX_PATH limits during package installation; the backend defaults to verified, in-process TypeScript anomaly engines (AdaptiveBaselineClassifier, ZScoreEngine, MedianDeviationEngine).

#### 6. Behavioral Fraud Detection and Risk Analytics (FraudGuard)
- **Repository**: [behavioral-fraud-detection-risk-analytics](https://github.com/NaraenderSoftware/behavioral-fraud-detection-risk-analytics)
- **Description**: A fraud detection and risk analytics prototype designed for zero-payment onboarding workflows (such as free tier and promotional signups). Evaluates passive client-side behavioral biometrics (completion time, mouse movement count, paste frequency, tab switches), SHA-256 device fingerprinting, IP velocity, and email intelligence (disposable domain detection, subaddress normalization) to compute an explainable composite risk score (0-100) and enforce a five-tier graduated decision model (ALLOW, MONITOR, CHALLENGE, REVIEW, BLOCK). Features automated fraud cluster detection for accounts sharing hardware or network identifiers, an administrative React console, and a standalone offline browser demonstration. Supported by 46 automated backend tests.
- **Technologies**: Python, Flask, React, Vite, SQLite, Behavioral Biometrics, Device Fingerprinting, Graph Clustering, REST APIs.
- **Verification Status & Documented Limitations**: The deterministic heuristics, behavioral telemetry analysis, and statistical Z-distance baseline anomaly fallback are fully implemented and verified with 46 passing tests. Real execution of the optional scikit-learn Isolation Forest model is unverified in the evaluated environment and relies on mocked branch tests. Database operations are verified against local SQLite with foreign-key enforcement; live PostgreSQL integration is implemented in code but unverified against an active server.

---

## Engineering Practices

- **Circuit Design & Prototyping**: Schematic capture, component derating, power budget verification, through-hole and surface-mount layout, manual wet-chemical board fabrication, and laboratory bench validation using oscilloscopes and digital multimeters.
- **Defensive Firmware Development**: Watchdog timers to prevent actuator burnout or link-loss runaways, atomic emergency stop routines across hardware pins and serial commands, input debouncing, and state-change display rendering.
- **Cross-Architecture Telemetry**: Packing and deserializing explicit binary structs across mixed processor architectures (RISC-V, Xtensa, and x86/ARM host environments) with byte-offset alignment to prevent padding errors.
- **Signal Processing & Statistical Analysis**: Time-domain vibration statistics (Peak, RMS, Crest Factor, fourth standardized moment Kurtosis), frequency-domain decomposition using Radix-2 FFT with Hann windowing, and robust non-parametric anomaly detection using Median and Median Absolute Deviation.
- **API Design & Data Ingestion**: REST and WebSocket streaming interfaces with strict physical range bounds checking, RFC 4180 CSV parsing, database transaction rollbacks, and administrative authorization controls.
- **Automated Verification & Auditing**: Automated unit testing with pytest and Jest/Vitest, repeatable firmware compilation audits via Arduino CLI, and clear documentation of system boundaries and unverified execution paths.

---

## GitHub and Organizations

- **Personal Profile**: [snaraender0937n](https://github.com/snaraender0937n)
- **Hardware Organization**: [NaraenderHardware](https://github.com/NaraenderHardware) - Case studies in PCB design, switched-mode power supplies, analog circuits, and embedded robotics.
- **Software Organization**: [NaraenderSoftware](https://github.com/NaraenderSoftware) - Distributed telemetry systems, industrial condition monitoring, and behavioral risk analytics.

---

## Contact

- **GitHub**: [https://github.com/snaraender0937n](https://github.com/snaraender0937n)
- **LinkedIn**: [https://www.linkedin.com/in/snaraender0937n/](https://www.linkedin.com/in/snaraender0937n/)
- **Portfolio Website (Intended)**: [https://snaraender0937n.github.io/naraender-portfolio/](https://snaraender0937n.github.io/naraender-portfolio/) (Deployment pending manual publishing)
- **Email**: snaraender@gmail.com

