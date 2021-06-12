Create RepicaSet by using below command

```
  kubectl create -f rs.yml
```  


kubectl also supports cascading deletion.

To delete dependents in the foreground using kubectl, set --cascade=foreground. To orphan dependents, set --cascade=orphan.

The default behavior is to delete the dependents in the background which is the behavior when --cascade is omitted or explicitly set to background.

Here's an example that orphans the dependents of a ReplicaSet:

```
  kubectl delete replicaset my-repset --cascade=orphan
```


```
  kubectl delete rs nodeapp
```  
  
  
