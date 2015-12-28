#WebJSnap Packer
This project houses a Packer (http://packer.io) template for building WebJSnap images.  The actual codebase for WebJSnap can be found at https://github.com/lamoni/webjsnap

#Currently Supported Builders
- VMWare
- Docker

# Instructions
- To build a VMWare image
```
packer build -only=vmware-iso webjsnap.json
```

- To build a Docker box
```
packer build -only=docker webjsnap.json
```

# Usage
- To access the WebJSnap frontend, just browse to the newly spun-up VM's IP address.  You should be able to "snapshot" any device on the same network as the VM (e.g. a vSRX running on the same host).
