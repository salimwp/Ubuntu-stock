This repo houses a basic Packer automation setup to build an Ubuntu 20.04 server.
Please change the username and password located in the httpd/user-data file. 
To create the image under QEmu use the following command:

```
packer build -force -only=qemu Ubuntu.json
```

For building an image for VirtualBox use the following command:
```
packer build -force -only=virtualbox-iso Ubuntu.json
```
