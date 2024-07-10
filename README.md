# ESP32-S3 1.28in. LCD Smartwatch

LOL this is of course completely not intended to be useful, I just want blinky lights.

## Setup
  Roughly Following: https://www.waveshare.com/wiki/ESP32-S3-Touch-LCD-1.28

1. Install Arduino IDE
2. Add https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json to the additional board url
3. Install the esp32 board from the boards manager (espressif not arduino is the publisher)
4. Restart Arduino IDE
5. Install the "TFT_eSPI" and "lvgl" libraries
6. Select the "ESP32S3 Dev Module" as the board
7. Change the flash size to "16MB (128Mb)"
8. Change the PSRAM to "QSPI PSRAM"

## Docs
Display API - https://www.waveshare.com/wiki/1.28inch_LCD_Module#Upper_application

<dl>
  <dt>Paint_*</dt>
  <dd>commands add to the current framebuffer image</dd>
  
  <dt>LCD_1IN28_Display</dt>
  <dd>Send the current framebuffer image to be rendered to the screen and then clears its contents to black</dd>
  
  <dt>LCD_1IN28_DisplayWindows</dt>
  <dd>Updates a specific region of the current screen with the matching region of the framebuffer. Then clears the framebuffer contents to black (the entire thing, not just the region specified)</dd>
</dl>
