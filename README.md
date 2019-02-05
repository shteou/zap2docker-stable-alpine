# zap2docker-stable-alpine

zap2docker-stable-alpine is an alpine based equivalent of the Ubuntu based
images provided by zaproxy/zaproxy, and is intended to be used in space
contrained systems

zap2docker-stable-alpine-minimal excludes several dependencies which are not
required by zaproxy for basic operation (e.g. VNC and firefox) leading to a
further reduction in image size

## Differences from Ubuntu base image

In using alpine as the base image, apk is used to install the dependencies.  
In addition, busybox is used, so useradd is replaced with busybox's adduser
function
