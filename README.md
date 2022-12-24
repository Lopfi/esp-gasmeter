# esp-gasmeter
An ESP32 with a reed switch that reads out a gas meter with a reed switch, triggered by a magnet in the last digit. Everything is written with the ESP-IDF. The ESP is in deep sleep most of the time and the ULP processor is counting the pulses. Every hour the ESP wakes up connects to wifi and sends the pulse count with an HTTP request to an influxdb with a grafana dashboard.
