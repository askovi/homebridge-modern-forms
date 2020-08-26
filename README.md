# Modern Forms Homebridge Plugin

Add [Modern Forms](https://modernforms.com) fans to your Home app using Homebridge.

## Prerequisites

- Have [Homebridge](https://homebridge.io) setup

## Setup

1. Add any devices you'd like to control to your home network.
    1. Download the Modern Forms [iOS](https://apps.apple.com/us/app/modern-forms/id1425046298) or [Android](https://play.google.com/store/apps/details?id=com.WAC.PlayStore.ModernForms&hl=en_US) app.
    1. Follow the instructions to pair your devices.
    1. Verify your devices show up in the app and can be controlled.
    1. Optionally, delete the app.

1. Add the following to your Homebridge `config.json` under platforms.

    ```json
        {
            "platform": "ModernForms"
        }
    ```

1. Verify your `config.json` looks similar to the following.

    ```json
    {
        "bridge": {
            "name": "Name",
            "username": "XX:XX:XX:XX:XX:XX",
            "port": 00000,
            "pin": "000-00-000"
        },
        "platforms": [
            {
                "platform": "ModernForms"
            }
        ]
    }
    ```

1. You’re all set! Any devices you saw in the Modern Fans app should appear in the Home app automatically.


