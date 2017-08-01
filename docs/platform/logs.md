# Introduction

D2C collects containerized applications' stdout to its own database. You can browse through logs any time in your dashboard. Keep in mind that your application should print logs to standard output for Docker daemon to be able to capture it and send it to our log facility.

There are three kinds of logs in D2C:

- **System logs** - deploy logs for each service
- **Container logs**
- **Host logs**

## System logs

Each service has system logs (deploy logs).

The line which has elision marks, in the end, can be opened with a mouse click.

![Build log](../img/build_log.png)

Messages of building images consist stdout, and it also can be shown.

![Stdout log](../img/stdout.png)

## Container logs

<!--нужно больше инфы (спросить у Паши)-->

Each container has logs. You may check them from the interface. [Read more](https://docs.docker.com/engine/admin/logging/view_container_logs/) about Docker logs.

![Container log](../img/containers_logs.png)

## Host logs

Each host has logs (server logs).

The line which has elision marks, in the end, can be opened with a mouse click.

![Host log](../img/host_logs.png)