# Troubleshooting
## Ubuntu command
1.<b> Q:</b>how to check the version of any ubuntu version </br>
<b> SolutionL:</b>lsb_release -a

## Ros
1. <b>Q:</b> Deployed multiple nodes on different machines, the published topic could be listed on the local one, 
also displayed on the other one. but "rostopic echo" dose not work for the other machine. </br>
<b>Solution:</b>adding all PCs with their hostnames and IP Adresses to the "/etc/hosts" file. Since then, everything works fine. 
## Ros Octomap
1. <b>Q:</b> How to use octomap to save the dataset in binary fromat. </br>
<b>Solution:</b>command line:  1. rosrun octomap_saver mapfile.bt" to request a compressed binary octomap via service call and save it to mapfile.bt.</br>
2. Run "octomap_saver -f mapfile.ot" to request a full probability octomap instead (Requires version 0.5 or later).</br>
