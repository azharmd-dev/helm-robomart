* Install the catalogue Helm chart using development-specific values
```
helm install catalogue . -f values-dev.yaml
```
* Updates the catalogue release to forward Service traffic to container port 80
```
helm upgrade catalogue . --set service.targetPort=80
```
