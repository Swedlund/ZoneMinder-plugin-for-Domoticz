# ZoneMinder-plugin-for-Domoticz
A Domoticz plugin that creates switches for each monitor configured on the ZoneMinder server and enables Domoticz to change their status

## Prerequisites
1. ZoneMinder API must be enabled, check out the API documentation (Wiki URL) for how to enable the API: http://zoneminder.readthedocs.io/en/stable/api.html
1. Rrequests libary for Python 3: https://pypi.org/project/requests/

## Installation
1. Clone repository into your Domoticz plugins folder
    ```
    cd domoticz/plugins
    git clone https://github.com/Frixzon/ZoneMinder-plugin-for-Domoticz.git
    ```
1. Restart domoticz
    ```
    sudo service domoticz.sh restart
    ```
1. Make sure that "Accept new Hardware Devices" is enabled in Domoticz settings
1. Go to "Hardware" page
1. Enter the Name
1. Select Type: `ZoneMinder`
1. Click `Add`

## Update
1. Go to plugin folder and pull new version
    ```
    cd domoticz/plugins/ZoneMinder-plugin-for-Domoticz
    git pull
    ```
1. Restart domoticz
    ```
    sudo service domoticz.sh restart
    ```

## Devices
The following devices are created:

| Type                | Name                      | Description
| :---                | :---                      | :---
| Selector Switch | Monitor #                     | Can set monitor state Monitor/Modect/Record/Mocord/Nodect
