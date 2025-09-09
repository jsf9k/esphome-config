# ESPHome Project #

This repository contains the ESPHome configurations for my home.

## Structure ##
- `devices/` → one YAML per device
- `packages/` → reusable config (WiFi, logging, base setup, etc.)
- `custom_components/` → optional ESPHome custom components
- `secrets.yaml` → **not checked in**, contains credentials
- `secrets.yaml.example` → template for secrets

## Usage ##
1. Clone this repo
2. `cd` into the repo
3. Copy `secrets.yaml.example` → `secrets.yaml` and fill in your WiFi and API secrets
4. Create a Python virtual environment:
   ```console
   pyenv virtualenv 3.13.7 esphome-config
   ```
5. Activate the Python virtual environment:
   ```console
   pyenv local esphome-config
   ```
6. Flash a device:
   ```console
   esphome run devices/skylight.yaml
   ```
