WG-Node-Red
===========

## Networkprinte MFC-8460N to WG-PI-FTP to Telegram

![help](img/telegram_druck_help.jpg)

![print](img/telegram_druck_print.jpg)

![pdf](img/telegram_druck_PdfList.jpg)

![tag](img/telegram_druck_tag.jpg)

## PI Sensor BME280

Man muss beim PI das Interface einschalten.

**01.** ``sudo raspi-config ``

**02.** Interfacing Options >> I2C >> enabled

**03.** ``sudo reboot``

---

Raspberry Pi 3 Model B+ Steckleiste ist SDA & SLC (i2c-1)

Um die Adresse zu finden kann man das Tool benutzen [npm install i2c-bus
](https://github.com/fivdi/i2c-bus)

```bash
i2cdetect -y <busnum>
```
![i2cadresse](img/BME280_I2Caddress.png)

---

![flowtest](img/BME280_FLOW.png)

npm install node-red-contrib-bme280

---

![dashboard](img/BME280_FLOW_02.png)