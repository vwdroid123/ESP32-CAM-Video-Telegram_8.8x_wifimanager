# ESP32-CAM-Video-Telegram_8.8x_wifimanager
ESP32-CAM-Video-Telegram

- Runs on ESP32-CAM AI-Thinker, stores video in SPIFFS - No need SD-Card!
- Record avi video on ESP32-CAM and send to Telegram on PIR/Motion (GPIO13) event or request
- WiFi manager to configure wifi credentials and telegram ID & AIP token by a PushButton GPIO12 (>=3sec), 1s = soft reboot
- Auto reconnect / reboot if wifi disconnected
- Fast blink - In config portal AP mode

Telegram commands:
-  /start
-  /photo - capture and send a photo
-  /flash - toggle flash led
-  /caption - photo with caption
-  /clip - send a photo followed by a short video clip AVI
-  /enable - enable pir
-  /disable - disable pir
-  /enavi - enable video capture
-  /disavi - disable video capture
-  /fast - 25fps play 0.5x speed
-  /med - 8fps play 1x speed
-  /slow - 2fps play 5x speed
-  /status
-  /reboot

Default settings:
-  15 second video AVI @ VGA
-  Frame_interval 125ms, play at real time 1x speed
-  PIR & AVI is always re-enabled on reboot

