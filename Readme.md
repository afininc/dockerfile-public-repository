## A-FIN I&C Dockerfile Public Repository

This repository contains the Dockerfiles for the A-FIN I&C Docker images. 

## Base Image

### node20-jre8-alpine-base

URL : public.ecr.aws/afininc/node20-jre8-alpine-base:latest

This image is Node.js 20 and OpenJDK jre 8 installed. 
It is based on Alpine Linux distribution (3.18 Version).


### node20-alpine-base

URL : public.ecr.aws/afininc/node20-alpine-base:latest

This image is Node.js 20 installed.
It is based on Alpine Linux distribution (3.18 Version).

## Template Image

### node20-jre8-ecs

This image using the node20-jre8-alpine-base image.
Sample Dockerfile for working at ECS.

### node20-ecs

This image using the node20-alpine-base image.
Sample Dockerfile for working at ECS.
