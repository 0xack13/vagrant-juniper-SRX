# vagrant-juniper-SRX
Running Juniper vSRX in Packet mode

## Install Vagrant pre-requisites
```
vagrant plugin install vagrant-host-shell
vagrant plugin install vagrant-junos
```

## Run the VMs
```
vagrant up
```

## Test the VMs 
```
vagrant ssh R1
# try and ping the other 192.x.x.x
sh int ter | match 192

# try from the other router as well
```
