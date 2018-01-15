# Kratos-c2-proxy

```
 | |/ /_ __ __ _| |_ ___  ___        ___|___ \ 
 | \' /| \'__/ _` | __/ _ \/ __|_____ / __| __) |
 | . \| | | (_| | || (_) \__ \_____| (__ / __/ 
 |_|\_\_|  \__,_|\__\___/|___/      \___|_____|
            

```

Kratos-C2 Proxy
---
The proxy is responsible for accepting requests for managing a node and a processing/relay commands.
The Proxy provides a REST API with Swagger Docs with the following:
* Authentication
* User name and password
* Permanent API key

* API Endpoints

* All CRUD operations for kratos_c2_proxy/models.py
* Command processor API endpoint (POST)

http://[hostname]/kratosc2/api/v1.0/

http://[hostname]/kratosc2/api/v1.0/MODEL_NAME

Kratos-c2 architecture (Open C2 concept)
----
```
C2 Client ------> C2 Proxy (Interface to C2 Master/Relay)
                       |        Setup node
                       |        Get Capabilities
                       |        Setup actuators
                       |        Setup capabilities
                       |
                       |
                    C2 Master <----->C2 Relay         (Orchestrator)Open C2 Capabilities/Sig Match
                                    |                   Dispatch cmds, load profiles
                                    |
                                    |
                                    |Control
                                    |
                                 Mitigation System Manager (orchestrator)
                                    |
                                    |
                                    |
                                 Actuators/Sensors
```                                 
