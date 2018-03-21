# Troubleshooting
## Ubuntu command
1.<b> Q:</b>how to check the version of any ubuntu version </br>
<b> SolutionL:</b>lsb_release -a

## Ros general issues
1. <b>Q:</b> Deployed multiple nodes on different machines, the published topic could be listed on the local one, 
also displayed on the other one. but "rostopic echo" dose not work for the other machine. </br>
<b>Solution:</b>adding all PCs with their hostnames and IP Adresses to the "/etc/hosts" file. Since then, everything works fine. 
## Ros Package Octomap
1. <b>Q:</b> How to use octomap to save the dataset in binary fromat. </br>
<b>Solution:</b>command line:  
1)."rosrun octomap_server octomap_saver map.bt" to request a compressed binary octomap via service call and save it to mapfile.bt.</br>
2). Run "octomap_saver -f mapfile.ot" to request a full probability octomap instead (Requires version 0.5 or later).</br>
## PCL
my ubuntu version is 16.04 LTS, after the install via apt-get command, I included the pcl tools into my source files, but after the cat_ kin compilation the problem occured.
 1. <b>Q:</b> /usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu/libpcl_common.so: undefined reference to 'GOMP_parallel@GOMP_4.0'fusion_octomap/CMakeFiles/OctoNode.dir/build.make:317: recipe for target '/home/kang/catkin_ws/devel/lib/fusion_octomap/OctoNode' failed</br>
<b>Solution:</b>command line:just follow the link to compile the pcl source and the install it locally. [install pcl and the Kinect support install](https://larrylisky.com/2014/03/03/installing-pcl-on-ubuntu/)
----command for qt version check: qtchooser -list-versions
## Datasets improvement for machine learning
[Datasets_improvement](https://hackernoon.com/stop-feeding-garbage-to-your-model-the-6-biggest-mistakes-with-datasets-and-how-to-avoid-them-3cb7532ad3b7?source=activity---post_recommended_rollup)

1. <b>Not enough data</b>
<b>Solution</b>Augment data via creating by slight variations or refine model;

2. <b>Low quality classes</b>
<b>Solution</b>Two stages classifications

3. <b>Low quality data</b>
<b>Solution</b>Means used to aquire data, build up dataset

4. <b>Unbalanced classes</b>
<b>Solution</b>Remove over-sample or augment the over-sample data

5. <b>Unbalanced data</b>
<b>Solution</b>Normalization

6. <b>No Validation for testing</b>
<b>Solution</b>Split

