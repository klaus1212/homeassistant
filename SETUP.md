# Home Assistant Setup

Encryptionkey: TKQC-88N0-70JY-45B8-2P9O-XK08-P4XN

## System Info
- **Device:** Synology DS218play
- **HA Version:** 2025.11.3-25 (SynoCommunity package)
- **IP:** 192.168.68.60:8123
- **SSH:** ehman@ds218play

## Inverter (SMA)
- **Lattitude, Longitude:** 54.91838390036865, 9.886179598483615
- **Type:** SMA Home Manager 2
  - **IP:** 192.168.68.66
- **Inverter** SMA hybrid inverter STP8.0-3SE-40
  - **IP:** 192.168.68.64
  - **Nominal PV power:** 12kwp
- **Battery:**
  - **Nominal battery capacity:** 12.8kwh
  - **Min SOC:** 25%
  - **Max SOC:** 100%
  - **Max charge capacity:** 10600w	
  - **Max discharge capacity:** 10600w
  - **BMS type:** Battery-Box Premium HVS	
- **Key Sensors:** 
  - Metering Total Yield (export)
  - Metering Total Absorbed (import)
  - Metering Power Supplied
  - Daily Yield
  - Battery SOC, Power, Charge/Discharge

## Energy Provider
- **Provider:** Norlys (DK1)
- **Nordpool Sensor:** sensor.nordpool_kwh_dk1_dkk_3_10_025
- **Unit:** øre/kWh

### Import Tariffs (øre/kWh)
- Energinet: 14
- Elafgift: 1
- Norlys Tillæg: 9.27
- Gridfee: 32.95 (time & season dependent)

### Export Tariffs (øre/kWh)
- Energinet Indfødningstarif: 0.5
- Energinet Balancetarif: 0.65
- Netselskab Indfødningstarif: 1.39
- Vindstød Balancetarif: 1

## File Paths
- **Config:** `/volume1/@appdata/homeassistant/config/configuration.yaml`
- **Log:** `/volume1/@appdata/homeassistant/config/homeassistant.log`
- **Git Repo:** https://github.com/klaus1212/homeassistant.git
- **Shared Folder:** `\\ds218play\homeassistant_config`

## Custom Sensors
### Price Sensors (øre/kWh)
- Nordpool Pris
- Elektricitet Import Pris per kWh
- Elektricitet Eksport Pris per kWh
- Elektricitet Månedlig Gennemsnitspris Import
- Elektricitet Månedlig Gennemsnitspris Eksport

### Cost/Revenue Sensors (DKK)
- Elektricitet Total Import Omkostning
- Elektricitet Total Eksport Indtægt

### Monthly Tracking
- Elektricitet Import Omkostning Måned
- Elektricitet Eksport Indtægt Måned
- Elektricitet Total Forbrugsmængde Måned
- Elektricitet Total Eksportmængde Måned

## Wheather forcast
- **Solcast:** https://solcast.com/
- **API key:** KClAHiTaL7XK4wqfeLUHghVsCOCsYDzl


## Additional Notes
*To be filled in...*
