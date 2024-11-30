<h3>Application of the NIST framework</h3>

|Summary	|The organization's internal network services suddenly stopped working due to a large number of incoming ICMP packets. Normal internal network traffic could not access any network resources. The incident management team then blocked incoming ICMP packets, stopped all non-critical network services offline, and restored critical network services. Investigation revealed that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This overwhelmed the company’s network through a distributed denial of service (DDoS) attack.|
|---------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Identify	|Network resources became inaccessible due to an incoming flood of ICMP packets by a malicious actor. The entire internal network was affected. All critical resources needed to be secured and restored to a functioning state. |
|Protect	|To address this security event, the network security team implemented a new firewall rule to limit the rate of incoming ICMP packets and an IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics.|
|Detect 	|To detect new unauthorized attacks in the future, the team implemented: </br>Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets.</br>Network monitoring software to detect abnormal traffic patterns.</br>IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics
|Respond  |The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. |
|Recover	|To recover from a DDoS attack by ICMP flooding, access to network resources need to be restored to a normal functioning state. In the future, a firewall can block ICMP flood attacks. Then, all non-critical network services should be stopped to reduce internal traffic. Next, critical services should be restored. Finally, after the flood of ICMP packets hace timed out, all non-critical network systems and services can be brought back online.|



Reflections/Notes: