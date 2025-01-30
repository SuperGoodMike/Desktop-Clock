# Desktop-Clock
Desktop-Clock Waveshare esp32-s3 Touch LCD 1.28 inches
# ESP32-S3 Touch LCD Weather Station

A MicroPython script for the Waveshare ESP32-S3 Touch LCD 1.28" that displays time, date, and local weather with touch interaction.

## Features
- Real-time weather display (temperature & humidity)
- Clock is geolocation-based time synchronization
- Touch-enabled temperature unit switching (°C/°F)
- Date and weekday display
- Automatic updates
- Wi-Fi connectivity

## Dependencies
- Waveshare micropython realease (found in `/MicroPython-bin` directory)
- Instructions on on how to flash micropython found here https://www.waveshare.com/wiki/ESP32-S3-Touch-LCD-1.28
- Fonts (stored in `/bitmap` directory)
- Touch driver cst816.py (stored in `/` directory)
- main.py and boot.py (stored in `/` directory)

## Hardware Requirements
- [Waveshare ESP32-S3-Touch-LCD-1.28](https://www.waveshare.com/wiki/ESP32-S3-Touch-LCD-1.28)
- Stable Wi-Fi connection
- USB-C cable for power/programming

## Configuration
1. Edit the following in the script:
   ```python
   # Wi-Fi credentials
   WIFI_SSID = "YOUR_WIFI_SSID"
   WIFI_PASSWORD = "YOUR_WIFI_PASSWORD"

## API Services Used
- IP-API.com (Geolocation)
- WorldTimeAPI.org (Time synchronization)
- Open-Meteo.com (Weather data)

## API configuration (api should work out of the box)
- GEOLOCATION_API_URL = "http://ip-api.com/json/"
- WORLD_TIME_API_URL = "https://worldtimeapi.org/api/timezone/{timezone}"
- WEATHER_API_URL = "http://api.open-meteo.com/v1/forecast..."

## Troubleshooting
- No display: Check SPI connections and backlight control
- Wi-Fi issues: Verify credentials and network stability
- API failures: Monitor serial output for error messages
- Touch unresponsive: Ensure proper initialization

## License
- MIT License - See LICENSE file

## Resources
- Waveshare Wiki https://www.waveshare.com/wiki/ESP32-S3-Touch-LCD-1.28
- MicroPython Documentation
- Open-Meteo API Docs

