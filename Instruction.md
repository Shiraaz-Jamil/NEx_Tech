Project Step : 1 Gathering information
Collecting Basic information about the following
1. The Internet of Things.
2. NodeMCU
3. Relay Module
4. Blynk application
5. IFTTT
6. Bridging
7. Arduino Programming

Step : 2 Equipment for the work
1. Active Wifi Connection
2. Laptop with Arduino IDE
3. NodeMCU
4. Relay Module
5. breadboard
6. Smartphone with Blynk app installed

Step : 3 Configuring Arduino IDE

Add NodeMCU board in your Arduino IDE
then,
In your Arduino IDE, go to File> Preferences
Enter "https://dl.espressif.com/dl/package_esp32_index.json, http://arduino.esp8266.com/stable/package_esp8266com_index.json" into the “Additional Boards Manager URLs” field as shown in the figure below. Then, click the “OK” button:
Then You will be able to find the ESP8266 library in Arduino's library manager
Then,
    In the Arduino IDE, navigate to Sketch > Include Library > Add .ZIP Library. At the top of the drop down list, select the option to "Add .ZIP Library''.
    Return to the Sketch > Include Library menu. menu. You should now see the library at the bottom of the drop-down menu. It is ready to be used in your sketch. The zip file will have been expanded in the libraries folder in your Arduino sketches directory.
Link of Zip - https://github.com/blynkkk/blynk-library/releases/tag/v0.6.1

Step-4 Preparing Power Source for NodeMCU

1.You can use the Data Cable
2.You can use 7-12 voltage battery.

Step : 5 Configuring the Blynk Application.

Install Blynk in your android or iOS phone.
login and you will see that a token key is being email to your registered E-mail id.
that token key is required in the code as well as in the IFTTT bridging.
after Dumping the code in the NodeMCU
You will see that your Blynk App recognized it  and declare it online.
after that add switches and other applets.
configure the pin which the respective pin you are using
And its ready to use

Step : 6 IFTTT bridging.

After testing out the code with Blynk App, now you can use the IFTTT bridging for connecting it with Alexa or Google Home or Assitant
Now you need to know that IFTTT have a large number of services from which you can do lots of things.
Open the drop-down menu.
select Create
Click IF
Select your A.I assistant.
Select your Phase
then Click on that
Select webhooks
URL:http://your country IP of Blink server /token/update/PIN
Method : Put
Content Type : application/json
Body : [“ (1 or 0 as per your On and Off configuration) ”], eg. ["1"]  .
You can find the Server IP of Blynk by typing ping blynk-cloud.com in your command prompt while connected to the internet.
The pinset is different in IFTTT for NodeMCU
 D0-D16
 D1-D5
 D2-D4
 D3-D0
 D4-D2
 D5-D14
 D6-D12 
 D7-D13
 D8-D15

then its done
and enjoy 

If there is any quieres contact me on Gitbit or E-mail me at zeshanrocks3@gmail.com
I am avalible between 5 pm to 7 pm of UTC +05:30(India)
