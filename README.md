#OpenRemote Controller

##Install On unRaid:

On unRaid, install container by adding bender77/openremote25

##Install On Other Platforms (like Ubuntu, Synology 5.2 DSM, etc.):

On other platforms, you can run this docker with the following command:

```
docker run -d --name="OpenRemoteController" --net="bridge" -p 8688:8688/tcp -v "/path/to/config":"/config":rw -v /etc/localtime:/etc/localtime:ro aptalca/docker-openremote
```

###Setup Instructions
- Replace the variable "/path/to/config" with your choice of folder on your system. That is where the config and the library files will reside, and they will survive an update, reinstallation, etc. of the container.
- To change the port, modify the port listed on the left side in the run command, that is the host side.
- Access the webui by going to http://SERVERIP:8688/controller
