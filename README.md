# IPMI tool for servers administration

## How to consume

```
git clone git@github.com:equinix-metal-use-cases/ipmi-tool.git
cd ipmi-tool
```

Start the Vagrant box

```
vagrant up --provider virtualbox
vagrant ssh
```

## Commands examples

create a SOL session

```
ipmitool -I lanplus -H 10.x.x.x -U <uname> -P <password> sol activate
```

destroy and activate SOL session

```
ipmitool -I lanplus -H 10.x.x.x -U <uname> -P <password> sol deactivate
```

reboot the server

```
ipmitool -I lanplus -H 10.x.x.x -U <uname> -P <password> power reset
```

reset BMC

```
ipmitool -I lanplus -H 10.x.x.x -U <uname> -P <password> bmc reset cold
```
