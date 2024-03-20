# 7 Attach storage Volumes to pods

## 7.1 Introducing volumes

Pod is like small logical computer. Containers share the computing resources but not file system. Only file in container is only those in the build. When the container stop all files will be gone. To continue from where we dropped off. We need the persist one. Adding the volume to the pod and mounting it into the container.

### How volumes fit into pods

Volumes are component of a pod so they share the same life cycle. Volume defined pod level and can be mounted at the container if desired.
