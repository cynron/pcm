--------------------------------------------------------------------------------
Instructions on How-To Run PCM Grafana Dashboard
--------------------------------------------------------------------------------

Installation on target system to be analyzed:
1.  Build: `make pcm-sensor-server.x`
2.  As root start pcm-sensor-server.x: `sudo ./pcm-sensor-server.x`


Installation of the grafana front-end (can be on any *host* system with connectivity to the target system):
1.  Make sure curl and docker are installed on the *host*
2.  In PCM source directory on the *host*: `cd grafana`
3.  (Download once and) start docker containers on the *host*: `sh start.sh http://target_system_address:80`
4.  Start your browser at http://*host*:3000/ and then login with admin user, password admin . Change the password and then click on "**Home**" (left top corner) -> "Processor Counter Monitor (PCM) Dashboard"
5.  You can also stop and delete the containers when needed: `sh stop.sh`
