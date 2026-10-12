# System Overview

## Problem and purpose

Aquaponics combines fish cultivation with plant growing in a shared water cycle. Changes in water quality, temperature, or water availability can affect the health of the system. EcoTrack's goal is to make relevant conditions easier to review in one place and to demonstrate how monitoring information could be organized for an operator.

## Current implementation

The existing project is a browser-based React dashboard. It includes overview, live-monitoring, historical-data, alerts, device-status, and settings views. The displayed measurements, samples, alerts, and device details are simulated frontend data. The dashboard itself labels its current state as demo mode with no ESP32 connected.

The current project does not include a device firmware package, a live sensor feed, a backend service, or a database connection. Physical hardware integration has not been demonstrated or tested as part of this showcase.

## Intended sensor and device roles

The following describes the intended system concept, not hardware already verified:

- **ESP32:** planned edge controller for reading compatible sensors and, in a future implementation, transmitting readings to a dashboard-facing service over a suitable connection.
- **pH sensor:** planned measurement of water acidity/alkalinity, useful for observing whether water conditions remain within chosen operating limits.
- **Water-temperature sensor:** planned measurement of the aquaponics water temperature.
- **Water-level sensor:** planned indication of water level or availability in the system.
- **Ambient temperature and humidity sensor:** planned context measurements for the environment around the aquaponics setup.

The frontend currently shows simulated values corresponding to these measurement categories. It does not establish that these specific sensors have been selected, wired, calibrated, or tested.

## Conceptual future data flow

`Sensors → ESP32 → future communications/service layer → dashboard`

The communications method, service, storage, security model, and deployment topology have not been finalized in the implementation represented here. They should be designed and validated before connecting real equipment or publishing real telemetry.
