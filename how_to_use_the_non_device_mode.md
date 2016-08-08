# 1. Creating New device with "Non Device" mode
First, you create a device in the "Non Device" mode

Although , the actual device is nothing, so you're finished setting the device name.

Launch the "IoT Gateway for BLE" app and tap the "New" button.

![introduce_gateway_app_ver_mqtt_add_ch1.png](https://lh3.googleusercontent.com/-SOyN_Sl3RuE/V5gRH97DP8I/AAAAAAAAJNE/0xi6nlTirHgZNfGvO6kWOrISh-MpjqlFwCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch1.png "introduce_gateway_app_ver_mqtt_add_ch1.png")

Tap the "Non Device" mode in a list.

![introduce_gateway_app_ver_mqtt_link_ch1.png](https://lh3.googleusercontent.com/-H5Z_YzUXbSY/V5gcwM40WNI/AAAAAAAAJOo/3bJ35oOrOA4nMccEQ5wWS3XI-vGwHrRVACKgB/s500/introduce_gateway_app_ver_mqtt_link_ch1.png "introduce_gateway_app_ver_mqtt_link_ch1.png")

Then you set the virtual device name your like, you will be appeared the screen to enter data.
You tap "Add" button then you have finished setting the name.

![introduce_gateway_app_ndm_add_dev1.png](https://lh3.googleusercontent.com/-Nd26qqhIECE/V5lfoAw1WrI/AAAAAAAAJWU/UT3OqppltLknm-mPFgX5TYzvJeZ2aYM4wCKgB/s500/introduce_gateway_app_ndm_add_dev1.png "introduce_gateway_app_ndm_add_dev1.png")

# 2. Linking a Channel
Next, you should link a device to the channel.

After you pressed the "Add" button in the edit screen of "Non Device" mode, It will be on the screen to select an existing channel list.

In this time, to make use of the MQTT channel that you created in the past.

Tap the MQTT channel in a list.

![introduce_gateway_app_ver_mqtt_add_ch2.png](https://lh3.googleusercontent.com/-3xQ5bDSCth8/V5gRN4SSFLI/AAAAAAAAJNU/kra4jTcdA4YUA_bIq5j9_EUzDP7tK6dtQCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch2.png "introduce_gateway_app_ver_mqtt_add_ch2.png")

And select the CloudMQTT broker that you created and then tap OK.

![introduce_gateway_app_ver_mqtt_link_ch7.png](https://lh3.googleusercontent.com/-8sedlrXQb7c/V5ge3XUgNTI/AAAAAAAAJQM/HN7N7XUOMe8Y1vu74lmNHK3Z6ySMzltmgCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch7.png "introduce_gateway_app_ver_mqtt_link_ch7.png")

To linking the MQTT channel and the "Non Device" device is now completed.
This operation will be the operation called as "Creating a Gateway" using "Non Device" mode.
Please check your gateway which has created in the list of Gateways.

![introduce_gateway_app_ndm_link_ch1.png](https://lh3.googleusercontent.com/-cKuPwMPZBvw/V5lfzCb-xtI/AAAAAAAAJWk/7YW9s2of3r008HAI87XSxUDYaMk96qJ7QCKgB/s500/introduce_gateway_app_ndm_link_ch1.png "introduce_gateway_app_ndm_link_ch1.png")

# 3. Test
So the last to try to test your gateway.
Please select the Gateway you created.

Tap the "Start" button then it will be shown the screen to start the Gateway.

![introduce_gateway_app_ver_mqtt_test1.png](https://lh3.googleusercontent.com/-lz9OmkA5Svk/V5gim2dbvJI/AAAAAAAAJQ0/yPC_03O5P1UMZziME2UMnCWgufFIYRmAwCKgB/s500/introduce_gateway_app_ver_mqtt_test1.png "introduce_gateway_app_ver_mqtt_test1.png")

It will start connection with MQTT cahnnel when starting the gateway.
There is no connection process with some device because the device does not exist in the "Non Device" mode actually.
To complete the connection to the MQTT channel, the Gateway is ready !
When the Gateway is ready, the "Do" button will be displayed at the top.

![introduce_gateway_app_ndm_test2.png](https://lh3.googleusercontent.com/-8DFP0tJ8Z7o/V5lf5uZhQJI/AAAAAAAAJW0/2bUfJ4bYQ6QqG-XwmMDV3kjnTD_-ECadQCKgB/s500/introduce_gateway_app_ndm_test2.png "introduce_gateway_app_ndm_test2.png")

You can send the data to MQTT channel using the "Do" button of your "Non Device".
Let's press the "Do" button.

![introduce_gateway_app_ndm_test3.png](https://lh3.googleusercontent.com/-Qrz5Fo_e39M/V5lgFhFce5I/AAAAAAAAJXE/6ICTwz6z-3IZRdboZWBd3NY2FfORWKOnwCKgB/s500/introduce_gateway_app_ndm_test3.png "introduce_gateway_app_ndm_test3.png")

For instance, it is a test that uses a mosquitto_sub command appears as follows:
In the case of "Non Device", the value ​​that are embedded in the {value} variable will be 0 at a fixed.

![introduce_gateway_app_ndm_test1.png](https://lh3.googleusercontent.com/-8Ohh7Ne1mrw/V5lcMB-U40I/AAAAAAAAJV8/bANcRRw-Oe0xosaqPEYZyRbcRQVoapK6ACKgB/s800/introduce_gateway_app_ndm_test1.png "introduce_gateway_app_ndm_test1.png")
