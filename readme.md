# PROTEUS

_protean: able to do many different things; versatile._

A high-featured board compatible with rusEfi firmware.

# Goals and Non-Goals

## Goals

- Run my LS-swapped Volvo 240 with factory harness and equipment
- Run a sequential ignition, quad-VVT v12 engine (twelve injectors, twelve ignition, five hall sensors, four VVT actuators, dual throttles)
- Easily manufactured sealed enclosure (all connectors mount in-plane)
- Extensible for knock sensing

## Non-goals

- Internal logging (doesn't make sense with 12 mbit/s USB, and a sealed enclosure)
- Direct injection
- Cheap

# Hardware Features

## Connectivity

- 1 mbit/s CAN bus
- USB 2.0 full speed (12 mbit/s), on-board or wired to connector for sealed applications

## Outputs
- 16x 4A low-side drivers
- 12x 5v ignition (or general purpose) outputs
- Dual H-bridges for electronic throttle (also supports stepper idle valve!)
- 4x 12v 3A high-side outputs

## Inputs

- 12x Analog voltage inputs
- 4x Analog temperature (5v pullup) inputs
- 2x VR crank/cam/vehicle speed inputs
- 6x hall cam/crank or digital input

## Power Supply

- Full operation from 6-24v supply
- Limited operation from 4-6v
- Dual 5v sensor supplies, 150mA each, fully protected
- ~~Dual protected 12v external sensor supply~~ TODO

## Extensibility

- 10-pin internal header for knock expansion board