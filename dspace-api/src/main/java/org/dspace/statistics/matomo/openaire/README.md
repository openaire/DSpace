
# OpenAIRE Matomo Event Listener Plugin

## Overview
In this [Pull Request](https://github.com/openaire/DSpace/pull/2), you will find implementation, which sends views & downloads events to OpenAIRE Matomo Statistics Service.
The implementation was done on DSpace v7.x, but it should work on v8.x, also. If your Dspace version is higher and this plugin doesn't work, please contact OpenAIRE to get support.
To integrate these changes into your DSpace repository, you can either cherry-pick PR's commit or just copy-paste all these files.

## Set Debug remote port on Docker
For remote debugging, the following values have been set in the docker-compose.yml. 
If you don't need to debug, you can undo these settings.
  
```
services:
    dspace:
        environment:
          CATALINA_OPTS: -Xmx2000m -agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=*:5005
    ports:
    - "5005:5005"
```
       
## Contact info:
```
repositoryusagestats@openaire.eu
```
