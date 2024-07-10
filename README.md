# BASH
#  For the 'ProtonVPNConnect'   
  Suppose you're like me, and tired of always inputing your your username and password on the command line, everytime you want to connect to your openvpn VPN server; Then this script is for you.
Usage: ./ProtonVPNConnect Path/filename.ovpn 
NOTE: Make sure you parse the full path to file

From your $HOME directory:
#  Clone the repository;
    git clone https://github.com/ostronic/BASH.git 
    cd BASH
    ll -t

# Edit the file using your favourite editor, to put in your username in the 
    sudo vi ProtonVPNConnectV2
# VPN_USER=username
and password in the 
# VPN_PASS=password 
space respectively, without quotes.

#  chmod/set the ACL to use without the bash command;
    sudo setfacl -m u:<username>:x ProtonVPNConnectV2
    ./ProtonVPNConnectV2 Path/filename.ovpn
    
#  Example: └──╼ $sudo ./ProtonVPNConnectV2 Downloads/us-free-628029.protonvpn.udp.ovpn
