# Introduction

D2C was designed to provide easy scaling for applications and hosts. Check your metrics online and use scaling when you need it. We are supporting horizontal scaling as well as vertical.

## Horizontal scaling

Horizontal scaling means increasing number of containers.
You can scale horizontal almost all [services](/getting-started/services/#native-support) in D2C. Open a service page and click **Scale**.

![Horizontal scaling](../img/horizontal_scaling.png)

Choose hosts which you want to be scaled to and click **Scale service**

![Horizontal scaling - choose hosts](../img/horizontal_scaling2.png)

After that, the scaling process starts, the status of service changes to *Scaling*. You can check system logs at the service page. The notification comes after the end of the process.

![Horizontal scaling - logs](../img/horizontal_scaling_logs.png)

## Vertical scaling

Vertical scaling means increasing power of a host (CPU, RAM). The process is quite easy - open a host page, choose the instance type and click **Resize**.

![Vertical scaling](../img/vertical_scaling.png)
