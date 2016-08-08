# 1. Registration CloudMQTT and making MQTT broker
Please create an account in CloudMQTT.

To regist an account is required e-mail address.

After you created an account, you have to make a broker.

It is OK if you can get information of the broker in CloudMQTT following as:
![introduce_gateway_app_ver_mqtt_broker.png](https://lh3.googleusercontent.com/-tizxPfRi-1U/V5gJV16cstI/AAAAAAAAJMc/puqZsrCMQXUkZIoPNgLmGwlUe-DVFAJ2wCKgB/s0/introduce_gateway_app_ver_mqtt_broker.png "introduce_gateway_app_ver_mqtt_broker.png")

You also have to add a user who can access topics of your broker.
![introduce_gateway_app_ver_mqtt_user.png](https://lh3.googleusercontent.com/-s27xsPMatzE/V5gJmUIkQyI/AAAAAAAAJMs/DSrCp7DjQz4lCS4Rdwn9V6XYqQsDJKHQACKgB/s800/introduce_gateway_app_ver_mqtt_user.png "introduce_gateway_app_ver_mqtt_user.png")

# 2. To register a broker info into the app
Next, you have to regist you created MQTT broker into the app.

Launch the "IoT Gateway for BLE" app and tap the "Channels" button.
![introduce_gateway_app_ver_mqtt_add_ch1.png](https://lh3.googleusercontent.com/-SOyN_Sl3RuE/V5gRH97DP8I/AAAAAAAAJNE/0xi6nlTirHgZNfGvO6kWOrISh-MpjqlFwCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch1.png "introduce_gateway_app_ver_mqtt_add_ch1.png")

Tap the MQTT channel in a list.
![introduce_gateway_app_ver_mqtt_add_ch2.png](https://lh3.googleusercontent.com/-3xQ5bDSCth8/V5gRN4SSFLI/AAAAAAAAJNU/kra4jTcdA4YUA_bIq5j9_EUzDP7tK6dtQCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch2.png "introduce_gateway_app_ver_mqtt_add_ch2.png")

And tap a "New" button in the bottom.
![introduce_gateway_app_ver_mqtt_add_ch3.png](https://lh3.googleusercontent.com/-ePCaU7G9tCo/V5gRUTaQXeI/AAAAAAAAJNk/8TZMh036aI0XCXpnDBpvmTUjb5UoBaB4QCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch3.png "introduce_gateway_app_ver_mqtt_add_ch3.png")

This will give you the chance to screen for entering the MQTT broker info. Input your broker info and the user info that you just created.

It is OK if you can input your broker data following as:
![introduce_gateway_app_ver_mqtt_add_ch4.png](https://lh3.googleusercontent.com/-vIkuS8fFwpo/V5gRaurcO8I/AAAAAAAAJN0/qKp7srOFzSokxO5xmIBrfUTaXq7AwXU_wCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch4.png "introduce_gateway_app_ver_mqtt_add_ch4.png")

Please try the "Connect Test".
If you can get the message of "Success Connect", it has been able to connect to the MQTT broker without problems.
![introduce_gateway_app_ver_mqtt_add_ch5.png](https://lh3.googleusercontent.com/-Z7QaNgPp6bQ/V5gSaeSqE7I/AAAAAAAAJOE/9tvG3zVIo4QWhELAg_HSv1rZh2zwIy97gCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch5.png "introduce_gateway_app_ver_mqtt_add_ch5.png")

Finally you tap the "Add" button, you have completed adding the new broker in  your MQTT channel.

To return to the list of MQTT channel then completed adding the new broker.
![introduce_gateway_app_ver_mqtt_add_ch6.png](https://lh3.googleusercontent.com/--14ujIoO158/V5gSo_b26SI/AAAAAAAAJOU/upnFDdf8HUYnQIPQWCXF0TFaQQcCReSRwCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch6.png "introduce_gateway_app_ver_mqtt_add_ch6.png")

# 3. Linking a Bluetooth device
Your bluetooth device is going to be linked to the MQTT channel that you created.

In this time, we chose one BLE device of "BLESerial2" made by ourself.

Anything is OK if a BLE device that supports the GATT Profile such as SensorTag.

Tap a "New" button in the Home.
![introduce_gateway_app_ver_mqtt_add_ch1.png](https://lh3.googleusercontent.com/-SOyN_Sl3RuE/V5gRH97DP8I/AAAAAAAAJNE/0xi6nlTirHgZNfGvO6kWOrISh-MpjqlFwCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch1.png "introduce_gateway_app_ver_mqtt_add_ch1.png")

And, tap a "BLE" button in the Device Mode.
Also, please turn ON the Bluetooth function on your smartphone.
![introduce_gateway_app_ver_mqtt_link_ch1.png](https://lh3.googleusercontent.com/-H5Z_YzUXbSY/V5gcwM40WNI/AAAAAAAAJOo/3bJ35oOrOA4nMccEQ5wWS3XI-vGwHrRVACKgB/s500/introduce_gateway_app_ver_mqtt_link_ch1.png "introduce_gateway_app_ver_mqtt_link_ch1.png")

To turn on the power of BLESerial2 device.
Then you should find a BLESerial2 in the "Device List".
![introduce_gateway_app_ver_mqtt_link_ch2.png](https://lh3.googleusercontent.com/-n9qZZq-S6us/V5gc-oXg54I/AAAAAAAAJO4/PTvKQocRphMg6g_JdcQJ7jsRcc78pkD2gCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch2.png "introduce_gateway_app_ver_mqtt_link_ch2.png")

Next, you should select a Service of you have selected the device.
![introduce_gateway_app_ver_mqtt_link_ch3.png](https://lh3.googleusercontent.com/-NYLwMId8cEU/V5gdHe3HTxI/AAAAAAAAJPI/ppekxwACZwA9NJSr6aTzT4XJPTlJwIMQgCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch3.png "introduce_gateway_app_ver_mqtt_link_ch3.png")

And next, you should select a Characteristic of you have selected the service.
Only supports "IoT Gateway for BLE" app in Notify type of Characteristic.
Because, it is necessary to receive the notification data from the BLE device in the app side.
To need to read on a regular basis the value from the application that it is Characteristic of the Read type.
Supports only Notify type for data that it is the case would continue to get the value even when not needed.
![introduce_gateway_app_ver_mqtt_link_ch4.png](https://lh3.googleusercontent.com/-xsMQwcHKx0w/V5geLVBK6XI/AAAAAAAAJPc/hgjtE8fBLtM3LZQQW6P0FtUztM6eF1W2ACKgB/s500/introduce_gateway_app_ver_mqtt_link_ch4.png "introduce_gateway_app_ver_mqtt_link_ch4.png")

You have selected the Notify type of Characteristic, please make sure not really a problem to tap the "Notify Test" button.
Add your BLE device tapping the "Add" button if there is no problem.
![introduce_gateway_app_ver_mqtt_link_ch5.png](https://lh3.googleusercontent.com/-kVqn9yMS0EI/V5geg5QZEkI/AAAAAAAAJPs/R1rCfC8CpJIg-PVvO-h_OdEVGIjLDsAGgCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch5.png "introduce_gateway_app_ver_mqtt_link_ch5.png")

This will give you the chance to screen to link a channel.
This time select the "MQTT" in a list, so you should link a BLE device to you just created MQTT channel.
![introduce_gateway_app_ver_mqtt_link_ch6.png](https://lh3.googleusercontent.com/-pG_2UE-RjS8/V5geuVO597I/AAAAAAAAJP8/lChVacdo2KIjo-jZYvfclvjHpHVIzJF5wCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch6.png "introduce_gateway_app_ver_mqtt_link_ch6.png")

And select the CloudMQTT broker that you created and then tap OK.
![introduce_gateway_app_ver_mqtt_link_ch7.png](https://lh3.googleusercontent.com/-8sedlrXQb7c/V5ge3XUgNTI/AAAAAAAAJQM/HN7N7XUOMe8Y1vu74lmNHK3Z6ySMzltmgCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch7.png "introduce_gateway_app_ver_mqtt_link_ch7.png")

To linking the MQTT channel and the BLE device is now completed.
This operation will be the operation called as "Creating a Gateway".
Please check your gateway which has created in the list of Gateways.
![introduce_gateway_app_ver_mqtt_link_ch8.png](https://lh3.googleusercontent.com/-I2pd_GEQxJ8/V5gfRWaTIqI/AAAAAAAAJQc/wiqTn4K4ch4GxLTAJqeoRjgCLfs3yp7lwCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch8.png "introduce_gateway_app_ver_mqtt_link_ch8.png")

# 4. Test
So the last to try to test your gateway.
Please select the Gateway you created.

Tap the "Start" button then it will be shown the screen to start the Gateway.
Power on your BLE device.
![introduce_gateway_app_ver_mqtt_test1.png](https://lh3.googleusercontent.com/-lz9OmkA5Svk/V5gim2dbvJI/AAAAAAAAJQ0/yPC_03O5P1UMZziME2UMnCWgufFIYRmAwCKgB/s500/introduce_gateway_app_ver_mqtt_test1.png "introduce_gateway_app_ver_mqtt_test1.png")

Search for BLE devices registered to start the Gateway, and has automatically connected to them.
It will start connection with MQTT cahnnel when the connection is completed with the BLE device.
And also completed the connection to the MQTT channel, the Gateway is ready !
![introduce_gateway_app_ver_mqtt_test2.png](https://lh3.googleusercontent.com/-TagJ6DVlu64/V5gisJEiQmI/AAAAAAAAJRE/VObDXL15zpsbRoOSLyBxl5SiZYtJI5EOgCKgB/s500/introduce_gateway_app_ver_mqtt_test2.png "introduce_gateway_app_ver_mqtt_test2.png")

When you send the data of Notify from BLE device, it will be published to the MQTT broker.
![introduce_gateway_app_ver_mqtt_test3.png](https://lh3.googleusercontent.com/-Cpe6g8w3X6g/V5giw_2SdZI/AAAAAAAAJRU/uq5gwL2gv3IiTf_25grhZrX_F7lKVHvxwCKgB/s500/introduce_gateway_app_ver_mqtt_test3.png "introduce_gateway_app_ver_mqtt_test3.png")

For instance, it is a test that uses a mosquitto_sub command appears as follows:
![introduce_gateway_app_ver_mqtt_test4.png](https://lh3.googleusercontent.com/-iSqysoDmWns/V5gjBAcP7TI/AAAAAAAAJRk/F-eYac6vmDsj2F39pfyYFTlHJoUGw0pZQCKgB/s800/introduce_gateway_app_ver_mqtt_test4.png "introduce_gateway_app_ver_mqtt_test4.png")
