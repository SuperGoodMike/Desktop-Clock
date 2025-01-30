# Desktop-Clock
Desktop-Clock Waveshare esp32-s3 Touch LCD 1.28 inches
# ESP32-S3 Touch LCD Weather Station

A MicroPython script for the Waveshare ESP32-S3 Touch LCD 1.28" that displays weather information, time, and date with touch interaction.

## Features
- Real-time weather display (temperature & humidity)
- Clock is geolocation-based time synchronization
- Touch-enabled temperature unit switching (°C/°F)
- Date and weekday display
- Automatic hourly weather updates
- Wi-Fi connectivity

## Dependencies
- Waveshare micropython realease https://www.waveshare.com/wiki/ESP32-S3-Touch-LCD-1.28
- Fonts (stored in `/bitmap` directory)
- Weather icons in JPG format (stored in `/jpg` directory)

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
   
   # API configuration (api should work out of the box)
   GEOLOCATION_API_URL = "http://ip-api.com/json/"
   WORLD_TIME_API_URL = "https://worldtimeapi.org/api/timezone/{timezone}"
   WEATHER_API_URL = "http://api.open-meteo.com/v1/forecast..."

