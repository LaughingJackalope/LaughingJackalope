# docker-desktop trinkets
This trinket is for the Docker Desktop Kubernetes cluster. It allows me to very quickly persist data to a local directory on  my mac when operating within the docker-desktop kubernetes context. 

## Caveat
These are my files, you'll need to adjust the paths to suit your own environment.

## Usage
```bash
# Create the storage class
kubectl apply -f storageClass.yaml
# Create the home persistent volume and claim
kubectl apply -f homepv.yaml
# Create the data persistent volume and claim
kubectl apply -f datapv.yaml
```

From this state you can now create a pod that uses the `home` or `data` persistent volume claims. The data written to these volumes will be on your local file system at the path specified in the `hostPath` of the `homepv.yaml` and `datapv.yaml` files.

## Cleanup
```bash
# Delete the home persistent volume and claim
kubectl delete -f homepv.yaml
# Delete the data persistent volume and claim
kubectl delete -f datapv.yaml
# Delete the storage class
kubectl delete -f storageClass.yaml
```