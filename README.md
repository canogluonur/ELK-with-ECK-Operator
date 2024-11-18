# ELK-with-ECK-Operator
ELK-with-ECK-Operator

first install these yaml

```
kubectl create -f https://download.elastic.co/downloads/eck/2.2.0/crds.yaml
```
and 
```
kubectl apply -f https://download.elastic.co/downloads/eck/2.2.0/operator.yaml
```
elastic password:
```
kubectl get secret -n logging elasticsearch-es-elastic-user -o=jsonpath='{.data.elastic}' | base64 --decode; echo
```
