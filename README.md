# fingerprint-scanner-system
Introduction: In this project we are designing a Biometric Attendance System using R307 fingerprint module and ESP32 board. This project uses IFTTT for storing fingerprints data along with the respective name of the person which is mentioned in the code of this project, to Google sheet which will be created automatically inside your Google drive and you can monitor the real time attendance on the go using your smartphone or laptop. With IFTTT, you don’t need to study about SQL and database or even you don’t need have your own website. This technique makes this project much easier to make and reliable as well.
What is IFTTT?
IFTTT is a free simple to use mobile app or website to make IOT projects. IFTTT derives its name from the programming conditional statement “if this, then that.” What the company provides is a software platform that connects apps, devices and services from different developers in order to trigger one or more automations involving those apps, devices and services
How does IFTTT work?
The automations are accomplished via applets — which are sort of like macros that connect multiple apps to run automated tasks. You can turn on or off an applet using IFTTT’s website or mobile apps (and/or the mobile apps’ IFTTT widgets). You can also create your own applets or make variations of existing ones via IFTTT’s user-friendly, straightforward interface. In this project, If event “Fingerprint” takes place, then add a row to Google drive’s spreadsheet is the applet used.
Components used: R307 fingerprint module, ESP32 dev board, breadboard, jumper wires
Circuit diagram: 



![image](https://github.com/pratyush-ec20/fingerprint-scanner-system/assets/78995911/c22c9622-e44f-4ac1-a05c-239bcf28863a)







Since the R307 fingerprint module works only in the range of 4.2v – 6v DC supply, the power is supplied from the Arduino uno board since the ESP32 board has no 5v pin. The ESP32 board is used to establish Wi-Fi connections and transfer data between fingerprint module and the app. The fingerprints are stored in the flash memory present in the R307 module
