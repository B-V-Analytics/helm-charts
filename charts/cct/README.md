
### Creating the registry pull secret
kubectl create secret docker-registry regcred -n cct --docker-server=ghcr.io --docker-username=<github username> --docker-password=<classic pat with read:packages scope> --docker-email=<placeholder mail> -o yaml --dry-run=client