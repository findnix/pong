# web pong
Pong running on Flask.

```
oc delete project rb-pong
sleep 10
oc new-project rb-pong
oc adm policy add-scc-to-user privileged -z default
oc new-app openshift/python~https://github.com/findnix/pong.git
oc expose service/pong
watch oc status
```
--> pip freeze > requirements.txt 
