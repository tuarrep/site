---
layout: project
title: Tunack
description: Kubernetes nginx ingress controller tcp/udp auto configuration
project: tunack
show_tile: true
---
## Motivation
When deploying lots of TCP or UDP custom services, it's needed to configure nginx ingress manager to bind port to these services. 
To do so it's needed to edit a configmap but usually this config isn't in the same namespace as the service and access may be restricted to the current user by cluster admin. 
tunack allows user to add an annotation to its service and automatically update nginx configmap in accordance.

## Technologies used
* golang
* Kubernetes golang API bindings
