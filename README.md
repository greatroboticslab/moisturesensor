# moisturesensor
What the Smart Box does
1) code connects to WiFI via the SSID and Password. Must be put into code at the moment
2) Automatically scans the WiFi for the proper channel to match it to ESP NOW
3) sends beacon to sensors to get them on the same channel so the box connects to the wifi and espnow at the same time
4) hosts a web server to view data via its IP address
5) updates SD card every minute
6) RTC has its own menue to reset it from the box
7) box is able to cycle between the different sensors

What the Sensor does
1) receives beacon from box so that ESP NOW and Wifi are all on the same channel
2) sends data to box every 15 minutes
3) sets channel based on box beacon
4) sensor number is set manually in the code, so each new sensor will need to have the number changed in the code before upload

Order of operations
1) plug box into wall outlet and the micro USB. Make sure USB is data only
2) watch serial output to ensure it connects to WiFi and gets an IP address
3) take note of the IP address
4) press the left and right buttons to get to the RTC menu
5) press right to check the date and time is correct, if not go back to the RTC menue and press left
6) if RTC was reset power box off then turn back on so that the file will have the proper time stamp
7) once box is botted and IP address is noted, USB can be unplugged
8) power on sensors
9) cycle through the sensors by pressing the middle button of the box to check the sensor is connected
10) go to a computer that is on the same wifi as the box, open the internet and type in the IP of the box. This opens a webpage displaying the data from the sensors
