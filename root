#!/bin/bash
# Simpel Change Root For Linux ( ALL LINUX OS )
# Auther = WildySheverando
# ================================================

# Clear
clear
rm -f root.sh

# Get Passwd
read -p "Please Input an New Password For Root : " Pass

# Starting Changes To Root
rm -f /etc/ssh/sshd_config
wget -O /etc/ssh/sshd_config https://raw.githubusercontent.com/wildysheverando-project/autoscript.github.io/main/sshd_config
echo -e "$Pass\n$Pass\n"|passwd root &> /dev/null
IPANDA=$(wget -qO- ifconfig.co);

# Successful
clear
echo "Please Save This VPS Account Information"
echo "============================================"
echo "  IP ADDRESS = $IPANDA"
echo "  Username   = root"
echo "  Password   = $Pass"
echo "============================================"
echo ""
echo "VPS Will Rebooting On 20 Second !!!!!"

rm -f root.sh
sleep 20
reboot
