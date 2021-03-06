# led-ring-clock
An Arduino-based analog clock using an WS2812B addressable RGB LED ring as a display.

This sketch requires the FastLED library, the Wire library (built-in), the EEPROM library (built-in), and the NtpClientLib.

https://github.com/FastLED/FastLED
https://github.com/gmag11/NtpClient/tree/develop

### 3D-printable enclosure
Design files available on Thingiverse: https://www.thingiverse.com/thing:2730265

### Electronics information
The LED ring is connected to digital pin 3. Momentary N/O button is connected to digital pin 5. 10K potentiometer is connected across power and ground and the wiper is connected to Analog 0. DS1307 RTC breakout is connected to the board's default I2C pins. This code has only been tested with an Adafruit 24 Neopixel Ring, but should (hopefully) work with any type or size of WS2812B ring, and with minimal changes it should work with rings using other types of RGB LEDs. The code should work on any ATmega328 based board.
