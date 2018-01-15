# Kratos-c2

```
 | |/ /_ __ __ _| |_ ___  ___        ___|___ \ 
 | \' /| \'__/ _` | __/ _ \/ __|_____ / __| __) |
 | . \| | | (_| | || (_) \__ \_____| (__ / __/ 
 |_|\_\_|  \__,_|\__\___/|___/      \___|_____|
            

```

Kratos-C2 is comprised of three main components

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
