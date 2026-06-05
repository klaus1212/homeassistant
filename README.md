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
- [done] feature/correct_pricing - get correct import (you buy) and correct export (you sell) price
- Prompt for setting up more intelligent battery charge.
	I want a daily wheather forecast and price forcast of electricity to control when my battery is charged.
	When my export price of electricity is high I want to export all of my PV production as possible and run my home on battery.
	Export price of electricity is found as Home Assistant sensor "Elektricitet Eksport Pris per kWh"
	When my export price of electricity is low I want to run my home on PV power and charge my battery with what is left.
	I want my battery fully charged using available PV power as predicted by whether forecast before sundown.
	If whether forecast shows enough PV power is available for my home and to charge my battery during a day I do not want to charge my battery from the grid.
	If there is not enough PV power available I only want to charge my battery from grid if sensor "Elektricitet Import Pris per kWh" is below 0,0 øre.


