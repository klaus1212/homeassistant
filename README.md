# Home Assistant Configuration

This repository contains my Home Assistant configuration for energy monitoring and cost calculation using Nordpool electricity prices and SMA inverter data.

## 📋 Documentation

- **[SETUP.md](SETUP.md)** - Complete system setup details including inverter specs, energy provider tariffs, and custom sensor configuration

## Tips and tricks

- From powershell ssh to synology
  ```
  ehman@ds218play:/usr$ sudo /usr/syno/bin/synopkg restart homeassistant
  Password:
  restart package [homeassistant] successfully
  ```

- Git from powershell
  - Add and commit
    ```
    git status          # list files that are modified
    git add             # add files to be committed
    git commit -m "..."  # commit message
    git push            # push to remote
    ```

  - Merge Squash
    ```
    cd "\\ds218play\homeassistant_config" && git branch -d feature/correct_pricing && git push origin --delete feature/correct_pricing
    ```

## Todo list
- [x] feature/correct_pricing - get correct import (you buy) and correct export (you sell) price
