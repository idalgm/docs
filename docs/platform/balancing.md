# Introduction

D2C supports load balancing provided by [HAProxy](http://www.haproxy.org/). It works in different modes: **HTTP**, **HTTPS**, **TCP**. The config generates automatically. All you need to do is open a service you need to balance and click **Add load balancer**.

## How to deploy a load balancer

1. Deploy or open a service you want to balance
2. Click **Add load balancer**
3. Choose a mode and a host
4. Click **Add load balancer**

If you use HTTPS HAProxy will be deployed with [Let's Encrypt](https://letsencrypt.org/) certificate (you may also add own certificate [after deploying](/platform/balancing/#edit-load-balancer)). Specify any additional ports if it needs. You may also disable access from the Internet (it is enabled by default).

![Load balancing](../img/balancing.png)

![Load balancing - mode and ports](../img/balancing_mode_ports.png)

![Load balancing - choose a host](../img/balancing_hosts.png)

## Edit load balancer

You may change a mode (config) after deploying. For this purpose open an HAProxy service, click **Edit settings**.

![Load balancing - editing](../img/balancing_editing.png)

Find a Configure services block and click on **Generate new config** icon.

![Load balancing - generate new config](../img/balancing_editing_new_config.png)

Choose a mode and click **Generate new config**.

![Load balancing - choose a mode](../img/balancing_editing_new_config_2.png)

If you need HTTPS, you may an add own certificate or use free automatically updated certificates provided by [Let's Encrypt](https://letsencrypt.org/).

Click **Update service**.

![Load balancing - update](../img/balancing_editing_update.png)