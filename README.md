# ESPHome Project #

This repository contains the ESPHome configurations for my home.

## Structure
- `devices/` → one YAML per device
- `packages/` → reusable config (WiFi, logging, base setup, etc.)
- `custom_components/` → optional ESPHome custom components
- `secrets.yaml` → **not checked in**, contains credentials
- `secrets.yaml.example` → template for secrets

## Usage
1. Clone this repo
2. Copy `secrets.yaml.example` → `secrets.yaml` and fill in your WiFi and API secrets
3. Flash a device:
   ```bash
   esphome run devices/skylight.yaml
