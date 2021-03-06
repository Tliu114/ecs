# Connect a Tier-0 Logical Router to a VLAN Logical Switch {#task_ppx_fhz_lgb .task}

This topic describes how to connect a tier-0 logical router to a VLAN logical switch to create an NSX Edge uplink.

-   Create a VLAN logical switch.
-   Create a tier-0 router.

1.  Open `https://nsx-manager-ip-address>` in your browser and log on to NSX Manager with your admin privileges. 
2.   Select **Routing** \> **Routers** and click the tier-0 logical router.![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/85014/154859278636133_en-US.png)

 
3.  Select **Configuration** \> **Router Ports** and click **ADD**. 
4.   Enter a name for the new tier-0 router port.![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/85014/154859278636134_en-US.png)

 
5.  Enter an optional description. 
6.  Select Uplink in the **Type** field. 
7.  Set the MTU size less or equal to 1500. 
8.  Select the Edge transport node from the drop-down menu. 
9.  Select Strict for the **URPF Mode**. URPF \(unicast Reverse Path Forwarding\) is a security feature. 
10. Select the VLAN logical switch from the drop-down menu. 
11. Select whether to attach the uplink router port to a new switch port or to an existing switch port. 
12. Type an IP address in CIDR notation in the same subnet as the connected port on the top of rack \(ToR\) switch. In this example, this IP address is the address of created **eni-ext** ENI that you can find in the ECS console. 

