title: Docker Workshop @ Hackafe
author:
  name: Rangel Ivanov
  twitter: mad_archer_
  github: https://github.com/ironsteel
output: kube.html

--
## 
<img src="https://insights.ubuntu.com/wp-content/uploads/8d9c/og_img.jpg"  heigth="100%" width="100%">


--

### Background

* Docker 
* Running docker in production ? 
  - Scaling
  - Loadbalancing
  - Service Discovery
  - Health checking
* Docker ecosystem (rival)
 
--

### What is kubernetes ? 

* Distributed process manager/scheduler
* Based on google borg 
   - http://research.google.com/pubs/pub43438.html
* Runs and manages containers on cluster of machines
* Deployment, Scaling etc

--

## 

<img src="https://mesosphere.com/wp-content/uploads/2015/09/k8s_architecture_overview.png"  heigth="100%" width="100%">


--


## 

<img src="http://severalnines.com/sites/default/files/kube7-arch.png"  heigth="100%" width="100%">


--


### Core components

* Pods
* Replication Controllers
* Selectors and labels
* Services

---

### Pods

* Collection of containers (one or more)
* Each pod gets it's own IP address
* Containers in a pod are interconected
* Ephemeral

---
### Labels and selectors

* Identify objects in the cluster
* Run queries and actions against the cluster
* Linking replication ctrls to pods 
* Linking services to pods/replication controllers

---

### Replication Controllers

* Replicates pods
* Rolling updates
* Keeps track of pods

---

### Services

* Defines logical set of pods 
* Abstracts access to pods
* Think microservice
* Service discovery
* Loadbalancer

---

### More

* Secret storage
* Persistant volumes
* Rolling updates
* Autoscaling
* Specify Resources (cpu, mem, disk) 
---

### Useful links

* http://kubernetes.io/
* Coreos - http://coreos.com/
  - Flannel
  - Etcd
  - Fleet
* Digital Ocean setup
  - https://github.com/charles-at-follow/do-k8s-playbooks

---

### And more...

* Kubernetes and cores using vagrant
  - https://coreos.com/kubernetes/docs/latest/kubernetes-on-vagrant.html
* Docker 
  - https://www.docker.com/
* Kubernetes PI
  - https://github.com/luxas/kubernetes-on-arm
