**Issue Summary:**
- **Duration:** May 10, 2024, 15:00 GMT to May 11, 2024, 03:00 GMT
- **Impact:** A significant portion of users (estimated 75%) experienced slow response times and intermittent downtime on our web platform.
- **Root Cause:** A misconfigured load balancer led to uneven distribution of traffic, causing server overload and subsequent performance degradation.

**Timeline:**
- **15:00 GMT:** Issue detected through monitoring alerts showing increased latency and error rates.
- **15:15 GMT:** Engineers investigated backend systems, suspecting database overload initially.
- **16:00 GMT:** Database team confirmed no anomalies, focus shifted to network infrastructure.
- **17:30 GMT:** Misleading assumption led to a thorough review of DNS settings.
- **18:45 GMT:** Issue escalated to senior network engineers for further investigation.
- **22:00 GMT:** Root cause identified as load balancer misconfiguration.
- **02:00 GMT:** Load balancer settings corrected, traffic redistributed evenly.
- **03:00 GMT:** Normal service resumed, with full system recovery.

**Root Cause and Resolution:**
The root cause of the issue was traced to a misconfigured load balancer, which failed to evenly distribute incoming traffic across backend servers. This resulted in certain servers being overloaded while others remained underutilized, causing performance degradation for users. The issue was resolved by correcting the load balancer settings to ensure proper traffic distribution, restoring system balance and functionality.

**Corrective and Preventative Measures:**
1. **Load Balancer Configuration Review:** Conduct a comprehensive review of load balancer configurations to identify and rectify any misconfigurations.
2. **Automated Monitoring:** Implement automated monitoring systems to detect and alert for uneven traffic distribution and server overload in real-time.
3. **Regular System Audits:** Schedule regular audits of network infrastructure and configurations to proactively identify and address potential issues before they impact user experience.
4. **Training and Documentation:** Provide additional training for engineers on troubleshooting methodologies and maintain up-to-date documentation on system configurations to facilitate efficient incident response in the future.

