## check_coiot_validator
Nagios compliant check to validate CoIoT JSON response from a Shelly device.

### Usage:

Query Device description via /cit/d

```
./check_coiot_validator -ip=192.168.178.210 -path=/cit/d
```

Query Status response via /cit/s

```
./check_coiot_validator -ip=192.168.178.210 -path=/cit/d
```

Example Response with /cit/d would be

```
OK: Payload is valid JSON
{"blk":[{"I":1,"D":"light_0"},{"I":2,"D":"device"}],"sen":[{"I":9103,"T":"EVC","D":"cfgChanged","R":"U16","L":2},{"I":1101,"T":"S","D":"output","R":"0/1","L":1},{"I":5101,"T":"S","D":"brightness","R":"0/100","L":1},{"I":5103,"T":"S","D":"colorTemp","U":"K","R":"2700/6500","L":1},{"I":5104,"T":"S","D":"whiteLevel","R":"0/100","L":1},{"I":4101,"T":"P","D":"power","U":"W","R":["0/9","-1"],"L":1},{"I":4103,"T":"E","D":"energy","U":"Wmin","R":["U32","-1"],"L":1}]}
```
