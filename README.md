# IPMI tool for servers administration

## How to consume

```
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
