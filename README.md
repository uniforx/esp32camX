# esp32camX
This is my adaption of the default ESP32 Cam Webserver with the LED Flash while streaming for monitoring my 3D printer in the dark.

# ATTENTION

While the camera image is being streamed via the URL "/stream", the LED for the flash is activated. This makes the module very hot and can damage it. This adaptation is NOT suitable for continuous operation! This is very important to know!!!

# Instructions

- Download and install Arduino IDE
- Go to “Menu > Preferences > Settings > Additional board manager URLs”. Add https://dl.espressif.com/dl/package_esp32_index.json in a new line and click OK.
- Restart Arduino IDE
- Connect your board to an USB port
- Install the required library by going to “Tools > Board > Boards Manager > Search for Esp32 > Install Esp32 from Espressif Systems”
- Select the correct Board “Tools > Board > ESP32 Arduino > AI Thinker ESP32-CAM” (maybe this can be another one)
- Burn this to the the board
- Search for the IP and open "http://192.168.0.xx:81/stream" for testing
