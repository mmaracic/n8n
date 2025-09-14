# Readme
https://github.com/n8n-io/n8n

## NPM local install
https://docs.n8n.io/hosting/installation/npm/

## Docker 

Created according to (steps 4+):  
https://docs.n8n.io/hosting/installation/server-setups/docker-compose/#2-optional-non-root-user-access

Run with:
```
docker-compose -f docker-compose.yml up|start
```

Application will be available at:
```
http://localhost:5678
```
## License
Licence received from n8n.io via email and activated in application (via Account->Settings->Usage and Plan->Enter Activation key).

## Concepts
Building own nodes or using community ones
https://docs.n8n.io/integrations/creating-nodes/overview/

Using external libraries (1st and 2nd answer)  
https://community.n8n.io/t/the-definitive-guide-to-custom-npm-modules-for-self-hosted-instances/50948/5

Concurrency  
https://docs.n8n.io/hosting/scaling/concurrency-control/


## Usual painpoints of flow automations (not confirmed here)
* deployment pattern (within application or standalone, custom functionality is inside or outside apps, how to scale, manage additional dependencies, estimate resources)
* edge cases
* error handling and recovery
* debugging
* no concurreny handling - offloaded downstream

## Observations
* No standard
* Deployed as node application presumably
* Can scale by additional horizontal deployments of worker nodes
* Can manipulate json data
* Can run javascript and some elementary python
* Has impressive number of integrations

## Questions
* Can it use external libraries?
* How general are extensions/templates, what can be added there?