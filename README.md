# ReadFish collector test

![](highLevelDiagram.svg)

## Steps
1. `podman pull docker.io/dmtf/redfish-mockup-server:latest`
1. `podman run --rm -p 8080:8000 dmtf/redfish-mockup-server:latest`
1. Call API

## API call examples
``` bash
curl -v http://localhost:8080/redfish/v1
curl -v http://localhost:8080/redfish/v1
curl -v http://localhost:8080/redfish/v1/Chassis
curl -v http://localhost:8080/redfish/v1/Chassis/1U
curl -v http://localhost:8080/redfish/v1/Chassis/1U/PowerSubsystem
```

# References
https://github.com/DMTF/Redfish-Mockup-Server
https://github.com/DMTF/Redfish-Mockup-Creator