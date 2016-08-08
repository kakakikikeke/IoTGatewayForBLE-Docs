# 1. To add an integration of Incomming Webhook
First, you have to add an integration of webhooks.

You can search "incoming webhook" in https://slack.com/apps.

Next, tap the "Add Configuration" button.

Input a channel in slack you want notify, and click the "Add Incoming Webhooks Integration".

Icon and name is whatever you want.

It will be OK. You could get a webhook URL following as:

![introduce_gateway_app_ver_slack_add_integration.png](https://lh3.googleusercontent.com/-G8N1p3ZPiRA/V5icIkzdE6I/AAAAAAAAJVg/FiHTlzEYuck3CPjSZnXzEOpFZDrQhpnlACKgB/s800/introduce_gateway_app_ver_slack_add_integration.png "introduce_gateway_app_ver_slack_add_integration.png")

# 2. To register the Slack info into the app
Next, you have to regist you created an incoming webhooks URL into the app.

Launch the "IoT Gateway for BLE" app and tap the "Channels" button.

![introduce_gateway_app_ver_mqtt_add_ch1.png](https://lh3.googleusercontent.com/-SOyN_Sl3RuE/V5gRH97DP8I/AAAAAAAAJNE/0xi6nlTirHgZNfGvO6kWOrISh-MpjqlFwCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch1.png "introduce_gateway_app_ver_mqtt_add_ch1.png")

Tap the Slack channel in a list.

![introduce_gateway_app_ver_mqtt_add_ch2.png](https://lh3.googleusercontent.com/-3xQ5bDSCth8/V5gRN4SSFLI/AAAAAAAAJNU/kra4jTcdA4YUA_bIq5j9_EUzDP7tK6dtQCKgB/s500/introduce_gateway_app_ver_mqtt_add_ch2.png "introduce_gateway_app_ver_mqtt_add_ch2.png")

And tap a "New" button in the bottom.

![introduce_gateway_app_ver_slack_add_ch1.png](https://lh3.googleusercontent.com/-PbJGfnz6Usk/V5iUF85hVoI/AAAAAAAAJSw/XtbEWZXw-Ck88cBvujoyUechduAbpRMIgCKgB/s500/introduce_gateway_app_ver_slack_add_ch1.png "introduce_gateway_app_ver_slack_add_ch1.png")

This will give you the chance to screen for entering the incoming webhooks info. Input the incoming webhooks data that you just created.

It is OK if you can input your broker data following as:

It is hard to enter a long string as Incoming Webhook URL in the iPhone.

Using an app that can share a data from PC, such as e-mail app and memo app will be information about the URL to easily input and to copy and paste.

![introduce_gateway_app_ver_slack_add_ch2.png](https://lh3.googleusercontent.com/-u00IPj8-UzY/V5iUlBFcHZI/AAAAAAAAJTA/rLYJM5KOFYkhqMMlTjmSDSzWQAKnIf6WgCKgB/s500/introduce_gateway_app_ver_slack_add_ch2.png "introduce_gateway_app_ver_slack_add_ch2.png")

Please try the "Connect Test".
If you can get the message of "Success Connect", it has been able to connect to the Slack channel without problems.

![introduce_gateway_app_ver_slack_add_ch3.png](https://lh3.googleusercontent.com/-qkdcx4y2wgk/V5iWLh6OHOI/AAAAAAAAJTY/LBBRDGYfpHoGuVawse4FFd4OwOILwa_XgCKgB/s500/introduce_gateway_app_ver_slack_add_ch3.png "introduce_gateway_app_ver_slack_add_ch3.png")

Finally you tap the "Add" button, you have completed adding the new Slack channel into the app.

To return to the list of Slack channel then completed adding the new data.

![introduce_gateway_app_ver_slack_add_ch4.png](https://lh3.googleusercontent.com/-QMEsbukgEAU/V5iWiiOB2bI/AAAAAAAAJTo/-j7pzxL2sSsHDghag2aInaf7-ptsb4CeQCKgB/s500/introduce_gateway_app_ver_slack_add_ch4.png "introduce_gateway_app_ver_slack_add_ch4.png")

# 3. Linking a Bluetooth device
Your bluetooth device is going to be linked to the Slack channel that you created.

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
This time select the "Slack" in a list, so you should link a incoming webhook of Slack channel you just created.

![introduce_gateway_app_ver_mqtt_link_ch6.png](https://lh3.googleusercontent.com/-pG_2UE-RjS8/V5geuVO597I/AAAAAAAAJP8/lChVacdo2KIjo-jZYvfclvjHpHVIzJF5wCKgB/s500/introduce_gateway_app_ver_mqtt_link_ch6.png "introduce_gateway_app_ver_mqtt_link_ch6.png")

And select the incoming webhooks of Slack that you created and then tap OK.

![introduce_gateway_app_ver_slack_link_ch1.png](https://lh3.googleusercontent.com/-XsfZFZ4r5DI/V5iZQ7TOk5I/AAAAAAAAJUE/BrtzZuUALjQt4V2EfmK8g0Kz5Foh92wvQCKgB/s500/introduce_gateway_app_ver_slack_link_ch1.png "introduce_gateway_app_ver_slack_link_ch1.png")

To linking the Slack channel and the BLE device is now completed.
This operation will be the operation called as "Creating a Gateway".
Please check your gateway which has created in the list of Gateways.

![introduce_gateway_app_ver_slack_link_ch2.png](https://lh3.googleusercontent.com/-jJLD-YOdYn4/V5iZpEi5gYI/AAAAAAAAJUU/QGPRmJkYTCEPpqSgU0Qu-SVz5qnHjhMbACKgB/s500/introduce_gateway_app_ver_slack_link_ch2.png "introduce_gateway_app_ver_slack_link_ch2.png")

# 4. Test
So the last to try to test your gateway.
Please select the Gateway you created.

Tap the "Start" button then it will be shown the screen to start the Gateway.
Power on your BLE device.

![introduce_gateway_app_ver_mqtt_test1.png](https://lh3.googleusercontent.com/-lz9OmkA5Svk/V5gim2dbvJI/AAAAAAAAJQ0/yPC_03O5P1UMZziME2UMnCWgufFIYRmAwCKgB/s500/introduce_gateway_app_ver_mqtt_test1.png "introduce_gateway_app_ver_mqtt_test1.png")

Search for BLE devices registered to start the Gateway, and has automatically connected to them.
It will start connection with Slack cahnnel when the connection is completed with the BLE device.
And also completed the connection to the Slack channel, the Gateway is ready !

![introduce_gateway_app_ver_slack_test1.png](https://lh3.googleusercontent.com/-b6qojaBReeY/V5iaiMbiRvI/AAAAAAAAJUo/jVZkD5IBYB0RoZq8zPFywmNlHRUhA7lrwCKgB/s500/introduce_gateway_app_ver_slack_test1.png "introduce_gateway_app_ver_slack_test1.png")

When you send the data of Notify from BLE device, it will be notified as messages to the specified Slack channel.

![introduce_gateway_app_ver_slack_test2.png](https://lh3.googleusercontent.com/-1DhyuaXyVIA/V5ibFpjFWkI/AAAAAAAAJU8/M8Y-Cg2wzOIpOOUB79V4laxnDkRI6Hh4gCKgB/s500/introduce_gateway_app_ver_slack_test2.png "introduce_gateway_app_ver_slack_test2.png")

Finally, you can verify that messages are notified to your channel of Slack following as:

![introduce_gateway_app_ver_slack_test3.png](https://lh3.googleusercontent.com/-QFu6rdhhcEY/V5ib0YqjfLI/AAAAAAAAJVQ/f-pLpRvUNnkbg-38yIQ2eqVoUguvt6YtwCKgB/s0/introduce_gateway_app_ver_slack_test3.png "introduce_gateway_app_ver_slack_test3.png")
