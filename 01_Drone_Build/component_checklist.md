# Drone F450 Component Checklist

This document tracks the components selected for the **Drone_F450 Forensics Research Project**.
The aim of this build is to create a Pixhawk-based F450 drone that can be used for learning UAV assembly, GPS-assisted flying, telemetry monitoring, flight-log collection, and forensic-style route reconstruction.

## Project Summary

The first version of this project focuses on building a stable drone platform using:

* F450 quadcopter frame
* Pixhawk 2.4.8 flight controller
* NEO-M8N GPS with compass
* FlySky remote-control system
* 3DR telemetry module
* Mission Planner ground station

Camera, live FPV, AI processing, and advanced sensors are kept for later phases. The first goal is to complete a safe and working drone that can generate useful flight logs for analysis.

---

## Main Drone Components

### F450 Frame Kit

The F450 frame is used as the base structure of the drone. It is large enough for beginner assembly, easy to repair, and suitable for mounting Pixhawk, GPS, telemetry, ESCs, and battery.

Included/selected:

* F450 frame
* A2212 1000KV brushless motors x 4
* 30A ESC x 4
* 1045 CW/CCW propellers

Extra 1045 propellers are also included because propellers are the most common parts to break during testing.

### Flight Controller

**Pixhawk 2.4.8 PX4 32-bit autopilot**

This is the main controller of the drone. It handles stabilization, GPS-assisted flight modes, failsafe, telemetry, and onboard flight logging.

It will be configured using **Mission Planner** with ArduPilot/ArduCopter firmware.

### GPS Module

**NEO-M8N GPS with compass and Pixhawk connector**

The GPS module is required for position hold, Loiter mode, Return-to-Launch, route tracking, and GPS-based forensic analysis.

### Remote Control System

**FlySky FS-i6X transmitter with FS-iA10B receiver**

This will be used to manually control the drone and switch between flight modes such as Stabilize, AltHold, Loiter, and RTL.

Frequency: **2.4GHz**

### Telemetry Module

**3DR Radio Telemetry 433MHz 500mW pair**

Telemetry allows the drone to send live flight data to the laptop through Mission Planner. This includes GPS position, altitude, flight mode, battery status, and warnings.

Frequency: **433MHz**

### Battery and Charger

Battery selected:

**11.1V 5200mAh 35C 3S LiPo battery**

Charger selected:

**iMax B6AC 80W smart balance charger**

The charger will be used in balance-charge mode for safe LiPo charging.

---

## Wiring and Electrical Items

The following items are selected for power wiring, soldering, and insulation:

* 100A power distribution board
* XT60 male-female connector pairs
* 14AWG red flexible silicone wire
* 14AWG black flexible silicone wire
* Heat shrink tube assorted kit
* 0.8mm rosin-core solder wire
* Electronics-grade flux paste

A basic digital multimeter will be arranged separately before first power-on. It is required to check voltage, polarity, and short circuits before connecting the LiPo battery.

---

## Tools and Assembly Items

The following tools and accessories are available or ordered:

* YIHUA 882D hot air and soldering station
* Agaro 115-piece precision screwdriver set
* Nylon cable ties
* Double-sided foam tape
* Battery Velcro ties/straps
* LiPo safety bag
* Medium-strength blue thread locker

These items will be used for clean wiring, safe soldering, component mounting, and battery securing.

---

## Camera Plan

Camera is not included in Phase 1.

The first version of the project will focus on:

* Drone assembly
* Pixhawk setup
* GPS lock
* Telemetry monitoring
* Flight log collection
* Route reconstruction

Camera, live FPV, SD-card recording, and AI-based visual analysis will be added later only after the drone is flying safely.

---

## Frequency Summary

* Remote control: **2.4GHz**
* Telemetry: **433MHz**
* Optional future FPV video: **5.8GHz**
* GPS: GNSS satellite signals through NEO-M8N module

---

## Phase 1 Goal

The first build version is:

**F450 + Pixhawk + GPS + Telemetry + Mission Planner**

The expected output from Phase 1 is a safe and working drone platform that can generate flight logs and GPS data for forensic-style analysis.

Main outputs:

* Stable drone assembly
* Mission Planner connection
* GPS lock verification
* Radio calibration
* Compass and accelerometer calibration
* Flight mode setup
* Telemetry monitoring
* Flight log download
* GPS route reconstruction

---

## Safety Notes

* Propellers must not be attached during setup or calibration.
* LiPo battery must not be connected until wiring polarity is checked.
* A multimeter must be used before first power-on.
* LiPo battery should be charged only in balance mode.
* LiPo safety bag should be used during charging and storage.
* Return-to-Launch and failsafe settings must be configured before outdoor flight.
