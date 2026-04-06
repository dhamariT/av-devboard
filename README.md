# av-devboard
**A custom PCB designed to be the brain of a small autonomous test vehicle.**

I'm from Detroit -- the Motor City. I spent time working out of Michigan Central Station, Ford's 30-acre innovation campus, as one of the first students in Google Code Next's Detroit lab. Being surrounded by Ford engineers and mobility startups every day showed me what the future of vehicles looks like -- and it's software-defined.

This project is my first dive into hardware. I'm designing a dev board from scratch around an STM32 microcontroller using KiCad. The goal is to build something that can actually drive motors, read sensors, and talk CAN bus like a real automotive ECU.

This is the hardware half of a bigger system. The other half is [ota-fleet-deployer](https://github.com/dhamariT/ota-fleet-deployer), an OTA update system I'm building in C++. The vision: the dev boards are the fleet, and the OTA system deploys firmware to them over the air. A fully self-built pipeline from silicon to deployment.

---

## Why I'm Building This

I'm targeting a career in autonomous vehicle software -- specifically Ford's Latitude AI. I want to understand the full stack, not just the software side. Building custom hardware gives me hands-on experience with the embedded systems, communication protocols, and real-time constraints that AV engineers deal with every day.

## What It Will Do

- **Motor Control** -- Drive motors via PWM for a small test vehicle platform
- **Sensor Fusion** -- Read an IMU (accelerometer + gyro) for vehicle state estimation
- **CAN Bus** -- Communicate using the automotive industry standard protocol
- **OTA Updates** -- Receive signed firmware updates from the ota-fleet-deployer system
- **Real-Time OS** -- Run everything on FreeRTOS so timing actually matters

## Status

This project is in early planning and research. I'm currently learning KiCad, studying STM32 datasheets, and prototyping firmware on a dev board before committing to custom hardware. The repo will grow as the build progresses.

## Related

- [ota-fleet-deployer](https://github.com/dhamariT/ota-fleet-deployer) -- The software side. OTA update system that will deploy firmware to these boards.

## License

MIT
