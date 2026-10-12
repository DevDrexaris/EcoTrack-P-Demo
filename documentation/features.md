# Dashboard Features

EcoTrack currently presents a frontend demonstration populated with simulated content. These descriptions refer to visible dashboard behavior and do not imply a live sensor connection.

## Overview

Shows a high-level summary of the simulated aquaponics readings and system state.

## Live Monitoring

Presents detailed simulated readings and recent samples for the measurement categories represented by the dashboard.

## Historical Data

Provides charts for reviewing demo trends across sensors and available time ranges.

## Alerts

Displays sample conditions such as readings outside configured demo limits. The interface supports acknowledging individual alerts and all alerts; acknowledgements are frontend state.

## Device Status

Shows simulated ESP32 node and connection information. It does not report the status of a connected physical device.

## Settings

Provides interface preferences, including the theme, and editable demo thresholds. These controls do not configure an external sensor or device.

## Navigation and accessibility

The application includes sidebar navigation between the six sections, URL-hash navigation state, and reduced-motion handling for the sidebar transition. Confirm behavior in the running app before relying on it in a live monitoring setting.
