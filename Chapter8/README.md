# Chapter 8 Persisting Volume and claims

## Why not just using persisting volume

The developer of the application must specify the google cloud or Amazon cloud persisting volume names. This means the kubernetes is not running on top of the cloud infrastructure instead is bound to it. The application should not care about where this application is deployed. so we use persistant volume with the claim.

### The persisting volume claim

![alt text](images/claim.png)

Instead of using the network Storage directly from the pod. You can use claim to direct to the volume. This way you can just use nfs system to point to the claim. You can just add the persistentVolumeClaim object that is bound to the PersistentVolume.
