The goal of fault management in telecom O&M (Operation & Maintenance) is to ensure stable & reliable networks and services. In the RAN (Radio Access Network), the most significant part of O&M activities is network fault management, including fault monitoring, analysis, diagnosis, and repair processes. Among these processes, fault analysis is an essential part of troubleshooting.

In the current practices with large-scale and complex network structure, O&M engineers have to face massive faults & alarms in daily work. The traditional way to analyze faults is by setting rules based on network experts’ experience, such as duration of faults or predefined categories of faults, to determine which faults need to be handled with higher priority.

However, with the traditional method, the impact of each fault on network KPIs (Key Performance Indicator), such as coverage and data rate, are not explicitly assessed and taken into consideration. As a result, the reliability of network service cannot be quantified and it is impossible to optimally schedule O&M resources. For example, even if some faults are so critical that NEs (Network Elements) are out of service because of them, they might not be urgent and could still be handled with lower priority. More precisely, consider a heterogeneous network where several NEs provide multiple layers of coverage (e.g., the co-existence of 4G and 5G, multiple frequency bands). In this case, even if a NE is out of service due to a sudden fault, there might not be coverage hole since users may migrate to neighboring NEs to access the network and obtain the same level of service quality. Therefore, the fault can be handled with low priority if other faults with worse impacts exist. In another case as stated in what follows, some faults need to be prioritized although they might only cause service capability deterioration of a NE rather than a service outage. When this kind of fault occurs, users can still access the network through the NE, but with a dropped service quality, which may lead to complaints and subscriber churn.

Problem statement In order to better guide fault management and optimally allocate limited O&M resources, this problem is targeting at leveraging ML/AI to predict the impact of faults on RAN KPIs. This is a critical capability for the autonomy of next-generation communications systems. It will empower the state-of-the-art fault management to upgrade from fixing network devices to fixing network service quality, and eventually drive network O&M transformation from equipment-centric to service-centric.

As described in the above examples, the impact of fault on RAN KPIs depend on network topology, NE’s historical and current running state and when & where the fault occurs. In the challenge, the participants are asked to develop a machine learning-based model to predict how each NE’s average data rate changes when a fault occurs based on network topology and historical data.
