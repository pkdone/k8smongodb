Guidance for running a [MongoDB](https://www.mongodb.com/) database cluster on the [Kubernetes](https://kubernetes.io/) orchestration framework, leveraging [Docker](https://www.docker.com/) containers. [StatetfulSets](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/) is a key dependency, to provide stable dedicated network storage volumes and hostnames, enabling data to outlive the lifetime of ephemeral containers. Note: The [MongoDB Operator for Kubernetes](https://docs.mongodb.com/kubernetes-operator/stable) incorporates these and other best practices in an easy to deploy way.

## Introduction To Running MongoDB on Kubernetes

1. [Deploying a MongoDB Replica Set as a Kubernetes StatefulSet](http://pauldone.blogspot.com/2017/06/deploying-mongodb-on-kubernetes-gke25.html)
2. [Configuring Some Key Production Settings for MongoDB on Kubernetes](http://pauldone.blogspot.com/2017/06/mongodb-kubernetes-production-settings.html)
3. [Using the Enterprise Version of MongoDB on Kubernetes](http://pauldone.blogspot.com/2017/06/enterprise-mongodb-on-kubernetes.html)
4. [Deploying a MongoDB Sharded Cluster using Kubernetes StatefulSets](http://pauldone.blogspot.com/2017/07/sharded-mongodb-kubernetes.html)
5. [MongoDB and Kubernetes Home Page](https://www.mongodb.com/kubernetes)
6. [MongoDB Operator for Kubernetes](https://www.mongodb.com/blog/post/introducing-the-mongodb-enterprise-operator-for-kubernetes) (by Robert Walters & Andrey Belik)


> WARNING: Some online resources advocate deploying a [sidecar](https://docs.microsoft.com/en-us/azure/architecture/patterns/sidecar), called [mongo-k8s-sidecar](https://lh4.googleusercontent.com/ohALxLD4Ugj5FCwWqgqZ4xP9al4lTgrPDc9HsgPWYRZRz_buuYK6LKSC7A5n98DdOO-Po3Zq77Yt43-QhTWdIaXqltHI7PX0zMXAXbpiilYgdowGZapG0lJ9lgubwBj1CwNHHtXA), to help "auto-configure" a MongoDB cluster. Do NOT employ that approach in Production environments, because this will result in [non-deterministic behaviour](http://pauldone.blogspot.com/2017/06/deploying-mongodb-on-kubernetes-gke25.html), adversely affecting database resiliency.

## Example Quickstart GitHub Projects

1. [Deploying a MongoDB Replica Set to the Google Kubernetes Engine (GKE)](https://github.com/pkdone/gke-mongodb-demo)
2. [Deploying a MongoDB Sharded Cluster to the Google Kubernetes Engine (GKE)](https://github.com/pkdone/gke-mongodb-shards-demo)
3. [Deploying a MongoDB Replica Set to the Azure Container Service (ACS)](https://github.com/pkdone/azure-acs-mongodb-demo)
4. [Deploying a MongoDB Replica Set to a local Minikube environment](https://github.com/pkdone/minikube-mongodb-demo)
5. [Deploying a MongoDB Replica Set to an OpenShift environment](https://github.com/pkdone/openshift-mongodb-demo)
6. [Deploying a MongoDB Replica Set to GKE Using MongoDB Cloud/Ops Manager](https://github.com/pkdone/k8s-cld-mgr)

## Getting Help on Stack Overflow

1. ["kubernetes" tagged questions](https://stackoverflow.com/questions/tagged/kubernetes)
2. ["google-container-engine" tagged questions](https://stackoverflow.com/questions/tagged/google-container-engine) or ["google-kubernetes-engine" tagged questions](https://stackoverflow.com/questions/tagged/google-kubernetes-engine)
3. ["azure-container-service" tagged questions](https://stackoverflow.com/questions/tagged/azure-container-service)
4. ["minikube" tagged questions](https://stackoverflow.com/questions/tagged/minikube)
5. ["openshift" tagged questions](https://stackoverflow.com/questions/tagged/openshift)
6. ["mongodb" tagged questions](https://stackoverflow.com/questions/tagged/mongodb)

> RECOMMENDED: When creating a new Stack Overflow question, define at least 2 tags: "mongodb" + a tag relating to the type of host Kubernetes environment.

## Useful Kubernetes Resources

1. [Kubernetes Manual](https://kubernetes.io/docs/concepts/)
2. [Kubernetes Up and Running book (Hightower, Burns & Beda - 2017)](https://www.amazon.co.uk/gp/product/B075G373MJ)
3. [Google Kubernetes Engine (GKE) for Kubernetes Manual](https://cloud.google.com/kubernetes-engine/docs/)
4. [Azure Container Service (ACS) for Kubernetes Manual](https://docs.microsoft.com/en-us/azure/container-service/kubernetes/)
5. [Minikube (Kubernetes locally) Manual](https://kubernetes.io/docs/getting-started-guides/minikube/)
6. [OpenShift with Kubernetes Manual](https://docs.openshift.org/latest/welcome/index.html)

## Useful Docker Resources

1. [Docker Manual](https://docs.docker.com/)
2. [Docker MongoDB Image Repository](https://hub.docker.com/_/mongo/)
3. [Docker MongoDB Image GitHub Project](https://github.com/docker-library/mongo) [(inc. building Enterprise version)](http://pauldone.blogspot.co.uk/2017/06/enterprise-mongodb-on-kubernetes.html)

## Useful MongoDB Resources

1. [MongoDB Manual](https://docs.mongodb.com/manual/)
2. [MongoDB and Kubernetes Home Page](https://www.mongodb.com/kubernetes)
3. [MongoDB Enterprise Kubernetes Operator](https://docs.mongodb.com/kubernetes-operator/stable)
4. [MongoDB Production Notes](https://docs.mongodb.com/manual/administration/production-notes/)
5. [MongoDB Operations Checklist](https://docs.mongodb.com/manual/administration/production-checklist-operations/)
6. [MongoDB Security Checklist](https://docs.mongodb.com/manual/administration/security-checklist/)

## Suggesting Changes To This Website

If you have a suggested change or addition to the content of this web page, please create a new "[issue](https://github.com/pkdone/k8smongodb/issues)", with a short description.
