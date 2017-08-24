Guidance for running [MongoDB](https://www.mongodb.com/) database clusters on the [Kubernetes](https://kubernetes.io/) orchestration framework, leveraging [Docker](https://www.docker.com/) containers. Fundamental to this is [Kubernetes StatetfulSets](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/), for stable dedicated network storage volumes and network hostnames, allowing data to outlive the lifetime of ephemeral containers.

## Introduction To Running MongoDB on Kubernetes

1. [Deploying a MongoDB Replica Set as a Kubernetes StatefulSet](http://pauldone.blogspot.com/2017/06/deploying-mongodb-on-kubernetes-gke25.html)
2. [Configuring Some Key Production Settings for MongoDB on Kubernetes](http://pauldone.blogspot.com/2017/06/mongodb-kubernetes-production-settings.html)
3. [Using the Enterprise Version of MongoDB on Kubernetes](http://pauldone.blogspot.com/2017/06/enterprise-mongodb-on-kubernetes.html)
4. [Deploying a MongoDB Sharded Cluster using Kubernetes StatefulSets](http://pauldone.blogspot.com/2017/07/sharded-mongodb-kubernetes.html)


> **WARNING**: Some online resource advocate deployment MongoDB using a [sidecar](https://docs.microsoft.com/en-us/azure/architecture/patterns/sidecar) called [mongo-k8s-sidecar](https://lh4.googleusercontent.com/ohALxLD4Ugj5FCwWqgqZ4xP9al4lTgrPDc9HsgPWYRZRz_buuYK6LKSC7A5n98DdOO-Po3Zq77Yt43-QhTWdIaXqltHI7PX0zMXAXbpiilYgdowGZapG0lJ9lgubwBj1CwNHHtXA) to help "auto-configure" a MongoDB cluster. Do NOT use such a mechanism in a Production environment because it will result in [non-determinisitc behaviour](http://pauldone.blogspot.com/2017/06/deploying-mongodb-on-kubernetes-gke25.html), adversly affecting the MongoDB cluster's availabiliy.

## Getting Help / Support

TODO

## Useful Kubernetes Resources

TODO

## Useful Docker Resources

TODO

## Useful MongoDB Resources

TODO: in prod checklists

## Suggesting Changes To This Site

If you have any suggested changes or additions to the content of this site, please raise create an [issue](https://github.com/pkdone/k8smongodb/issues) with a short description.


## TODO

* k8s/mongo image in top left (merge 2 icons)
* talk about gke, azure, openshift, local instal, etc
