# Testing IoTSemplice

### Required materials

* One [IoTSemplice](http://www.iotsemplice.com/) main board
* One microswitch connected to Digital Input 0
* One LED connected to Digital Output 3
* One Android smartphone

### Step-by-step instructions

* TODO: Wiring instructions for microswitch and LED
* Install Android App [nRF Master Control Panel](https://play.google.com/store/apps/details?id=no.nordicsemi.android.mcp&hl=it) to smartphone
* Start App "nRF Master Control Panel"

Inside "nRF Master Control Panel", tap **SCANNER**.

- Identify the entry for your iBLIO (example: xxx)
- Tap **CONNECT**


* Characterstic `xxx1000`
* UUIF `xxxx-2901-xxx` (OUT3)
* Tap **Up Arrow***

* Type: `UINT16`
* Value: (enter a value between 0 and 65535)
  - 0: LED off
  - 1 < _n_ < 65535: Turn on led for _n_ seconds
  - 65535: LED always on

TODO

<!-- EOF -->
