---
pcx-content-type: concept
title: Standard
weight: 1
---

# Standard steering policies

Standard steering policies include **Off - standard failover** and **Random**.

These are the only steering policies available to non-Enterprise customers who have not purchased **Traffic Steering**.

## Off - standard failover

Standard failover directs traffic from unhealthy pools — determined by [health checks](/load-balancing/understand-basics/monitors/) and the **Health Threshold** — to the next healthy pool in the configuration. Customers commonly use this option to set up [active - passive failover](/load-balancing/reference/common-configurations/#active---passive-failover).

Standard failover uses the pool order to determine failover priority (the failover order).

If all pools are marked unhealthy, Load Balancing will direct traffic to the fallback pool. The default fallback pool is the last pool listed in the Load Balancing configuration.

If no monitors are attached to the load balancer, it will direct traffic to the primary pool exclusively.

## Random steering

Choose **Random** to route traffic to a healthy pool at random. Customers can use this option to set up [active - active failover](/load-balancing/reference/common-configurations/#active---active-failover) (also known as round robin), where traffic is split equally between multiple pools.