#Troubleshooting
##ubuntu command
1.<b> Q</b>how to check the version of any ubuntu version </br>
<b> Solution</b>lsb_release -a

##ubuntu command
1. <b> Q</b> Deployed multiple nodes on different machines, the published topic could be listed on the local one, 
also displayed on the other one. but "rostopic echo" dose not work for the other machine. </br>
<b> Solution</b>adding all PCs with their hostnames and IP Adresses to the "/etc/hosts" file. Since then, everything works fine. 
