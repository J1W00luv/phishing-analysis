# Learning and Understanding Phishing Links

## **Aim:**
	To understand how phishing links are created using Storm-Breaker and how the data can be stolen through the network tunnels created by NGROK. To analyze the results afterwards and understand how phishing type of attacks could be prevented.

## **Method:**
	* 1. Set up the controlled environment: Configure Kali Linux VM and install Storm Breaker.
	* 2. Prepare tunnels: Use NGROK to create safe network tunnels
	* 3. Attack simulation: Create testing phishing URLs, preparing for the data capture.
	* 4. Data capture & analysis: Use the test URL on mobile devices and identify Indicators of Compromise.

Problems i had during the execution:

## **Problems occurred & Solutions**

Problem | Description | Solution
Installation path failure | A failure occurred during the NGROK installation process, due to the incorrect relative path execution. | I used the absolute path to move files to the correct system location.

Network blocking | During the testing data capture process failed due to the mobile operator’s defensive mechanism blocking the attack. | I used local WiFi over cellular data.



## **Testing Results:**
	All three tests performed as expected, proving the effectiveness of the attack on different operating systems(IOS & Android) and both inside and outside of the WiFi network which my PC was connected to. However, data capturing was heavily relied on the unencrypted HTTP data ports (eg. 2525). On one of my tests the mobile operator proved to block the connection, not allowing the data to be stolen. It is suggested that it already had a good defence system against phishing attacks.

## **Conclusion:**
	In this practical I have simulated the life cycle of a phishing attack. I have learned about highly efficient phishing tools (“Storm-Breaker”, and “NGROK”) and how the data can be captured through the network tunnels. The key Indicators of Compromise included use of HTTP ports (2525), which are not considered secure. The defence against those types of attacks highly rely on user education and detection systems, which should be able to detect and block this type of network traffic.

