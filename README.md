Heart Rate and Temperature Monitoring with MAX30102 Sensor

This Python script is designed to run on a microcontroller with an ESP32 chip and a MAX30102 sensor for heart rate and temperature monitoring. 
It connects to a WiFi network and publishes the data to Adafruit IO via MQTT.

    Prerequisites:
      Microcontroller with an ESP32 chip
      MAX30102 sensor
      WiFi network credentials (SSID and password)
      Adafruit IO account with the credentials (username and API key)

    Dependencies:
      umqtt.robust: MQTT client library for MicroPython
      machine: MicroPython module for hardware control
      utime: MicroPython module for time-related functions

    Installation:
      1. Clone this repository to your local machine:
        git clone https://github.com/your-username/your-repo.git
      
      2. Connect the MAX30102 sensor to your microcontroller board according to the pin configuration specified in the code.
      3. Update the following variables in the code with your WiFi credentials and Adafruit IO details:
        WIFI_SSID = 'YourWiFiSSID'
        WIFI_PASSWORD = 'YourWiFiPassword'

        ADAFRUIT_USERNAME = 'YourAdafruitUsername'
        ADAFRUIT_IO_KEY = 'YourAdafruitIOKey'

      4. Upload the code to your microcontroller board.

    Setup
      Connect the MAX30102 sensor to the microcontroller.
      Update the WiFi network credentials (WIFI_SSID and WIFI_PASSWORD) in the script.
      Update the Adafruit IO credentials (ADAFRUIT_USERNAME and ADAFRUIT_IO_KEY) in the script.

    Usage

      Upload the script to the microcontroller.
      Power on the microcontroller.
      The script will connect to the WiFi network and Adafruit IO.
      It will continuously monitor heart rate and temperature using the MAX30102 sensor.
      Data will be published to Adafruit IO at regular intervals.
      You can view the data on the Adafruit IO dashboard by logging into your Adafruit IO account.
