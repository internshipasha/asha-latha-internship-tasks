Network Scan Project

This project demonstrates the use of Nmap/Zenmap for network scanning.

Tools Used

Nmap (command-line)

Zenmap (GUI for Nmap)


Methodology

1. Attempted a full TCP scan on all 65,535 ports across the subnet x.x.1.x-254 using:

nmap -p 1-65535 -T4 -A -v x.x.x.x-x

This scan was very large and took a long time to complete.
2. Saved partial results from Zenmap after several hours of scanning.

Example: some hosts (e.g., 192.168.1.5, 192.168.1.14) showed open ports such as 80, 443, 8009, 8080, 3306.



3. Learned that in real environments, it is better to:

Limit scans to top 1000 ports (default Nmap behavior), or

Scan specific ports (e.g., 22, 80, 443, 3306) for faster results.




Results

The raw scan output is saved in <?xml version="1.0" encoding="utf-8"?>
<?xml-stylesheet href="file:///C:/Program Files (x86)/Nmap/nmap.xsl" type="text/xsl"?><nmaprun args="nmap -p 1-65535 -T4 -A -v 192.x.x.x-254" profile_name="Intense scan, all TCP ports" scanner="nmap" start="1758518863" startstr="Mon Sep 22 10:57:43 2025" version="7.97" xmloutputversion="1.04"><scaninfo type="syn" protocol="tcp" numservices="65535" services="1-65535"></scaninfo><verbose level="1"></verbose><debugging level="0"></debugging><output type="interactive">Starting Nmap 7.97 ( https://nmap.org ) at 2025-09-22 10:57 +0530
NSE: Loaded 158 scripts for scanning.
NSE: Script Pre-scanning.
Initiating NSE at 10:57
Completed NSE at 10:57, 0.00s elapsed
Initiating NSE at 10:57
Completed NSE at 10:57, 0.00s elapsed
Initiating NSE at 10:57
Completed NSE at 10:57, 0.00s elapsed
Initiating ARP Ping Scan at 10:57
Scanning 253 hosts [1 port/host]
Completed ARP Ping Scan at 10:57, 6.28s elapsed (253 total hosts)
Initiating Parallel DNS resolution of 253 hosts. at 10:57
Completed Parallel DNS resolution of 253 hosts. at 10:59, 102.62s elapsed
Nmap scan report for 192.168.1.6 [host down]
Nmap scan report for 192.168.1.7 [host down]
Nmap scan report for 192.168.1.9 [host down]
Nmap scan report for 192.168.1.10 [host down]
Nmap scan report for 192.168.1.11 [host down]
Nmap scan report for 192.168.1.12 [host down]
Nmap scan report for 192.168.1.13 [host down]
Nmap scan report for 192.168.1.14 [host down]
Nmap scan report for 192.168.1.15 [host down]
Nmap scan report for 192.168.1.16 [host down]
Nmap scan report for 192.168.1.17 [host down]
Nmap scan report for 192.168.1.18 [host down]
Nmap scan report for 192.168.1.19 [host down]
Nmap scan report for 192.168.1.20 [host down]
Nmap scan report for 192.168.1.21 [host down]
Nmap scan report for 192.168.1.22 [host down]
Nmap scan report for 192.168.1.23 [host down]
Nmap scan report for 192.168.1.24 [host down]
Nmap scan report for 192.168.1.25 [host down]
Nmap scan report for 192.168.1.26 [host down]
Nmap scan report for 192.168.1.27 [host down]
Nmap scan report for 192.168.1.28 [host down]
Nmap scan report for 192.168.1.29 [host down]
Nmap scan report for 192.168.1.30 [host down]
Nmap scan report for 192.168.1.31 [host down]
Nmap scan report for 192.168.1.32 [host down]
Nmap scan report for 192.168.1.33 [host down]
Nmap scan report for 192.168.1.34 [host down]
Nmap scan report for 192.168.1.35 [host down]
Nmap scan report for 192.168.1.36 [host down]
Nmap scan report for 192.168.1.37 [host down]
Nmap scan report for 192.168.1.38 [host down]
Nmap scan report for 192.168.1.39 [host down]
Nmap scan report for 192.168.1.40 [host down]
Nmap scan report for 192.168.1.41 [host down]
Nmap scan report for 192.168.1.42 [host down]
Nmap scan report for 192.168.1.43 [host down]
Nmap scan report for 192.168.1.44 [host down]
Nmap scan report for 192.168.1.45 [host down]
Nmap scan report for 192.168.1.46 [host down]
Nmap scan report for 192.168.1.47 [host down]
Nmap scan report for 192.168.1.48 [host down]
Nmap scan report for 192.168.1.49 [host down]
Nmap scan report for 192.168.1.50 [host down]
Nmap scan report for 192.168.1.51 [host down]
Nmap scan report for 192.168.1.52 [host down]
Nmap scan report for 192.168.1.53 [host down]
Nmap scan report for 192.168.1.54 [host down]
Nmap scan report for 192.168.1.55 [host down]
Nmap scan report for 192.168.1.56 [host down]
Nmap scan report for 192.168.1.57 [host down]
Nmap scan report for 192.168.1.58 [host down]
Nmap scan report for 192.168.1.59 [host down]
Nmap scan report for 192.168.1.60 [host down]
Nmap scan report for 192.168.1.61 [host down]
Nmap scan report for 192.168.1.62 [host down]
Nmap scan report for 192.168.1.63 [host down]
Nmap scan report for 192.168.1.64 [host down]
Nmap scan report for 192.168.1.65 [host down]
Nmap scan report for 192.168.1.66 [host down]
Nmap scan report for 192.168.1.67 [host down]
Nmap scan report for 192.168.1.68 [host down]
Nmap scan report for 192.168.1.69 [host down]
Nmap scan report for 192.168.1.70 [host down]
Nmap scan report for 192.168.1.71 [host down]
Nmap scan report for 192.168.1.72 [host down]
Nmap scan report for 192.168.1.73 [host down]
Nmap scan report for 192.168.1.74 [host down]
Nmap scan report for 192.168.1.75 [host down]
Nmap scan report for 192.168.1.76 [host down]
Nmap scan report for 192.168.1.77 [host down]
Nmap scan report for 192.168.1.78 [host down]
Nmap scan report for 192.168.1.79 [host down]
Nmap scan report for 192.168.1.80 [host down]
Nmap scan report for 192.168.1.81 [host down]
Nmap scan report for 192.168.1.82 [host down]
Nmap scan report for 192.168.1.83 [host down]
Nmap scan report for 192.168.1.84 [host down]
Nmap scan report for 192.168.1.85 [host down]
Nmap scan report for 192.168.1.86 [host down]
Nmap scan report for 192.168.1.87 [host down]
Nmap scan report for 192.168.1.88 [host down]
Nmap scan report for 192.168.1.89 [host down]
Nmap scan report for 192.168.1.90 [host down]
Nmap scan report for 192.168.1.91 [host down]
Nmap scan report for 192.168.1.92 [host down]
Nmap scan report for 192.168.1.93 [host down]
Nmap scan report for 192.168.1.94 [host down]
Nmap scan report for 192.168.1.95 [host down]
Nmap scan report for 192.168.1.96 [host down]
Nmap scan report for 192.168.1.97 [host down]
Nmap scan report for 192.168.1.98 [host down]
Nmap scan report for 192.168.1.99 [host down]
Nmap scan report for 192.168.1.100 [host down]
Nmap scan report for 192.168.1.101 [host down]
Nmap scan report for 192.168.1.102 [host down]
Nmap scan report for 192.168.1.103 [host down]
Nmap scan report for 192.168.1.104 [host down]
Nmap scan report for 192.168.1.105 [host down]
Nmap scan report for 192.168.1.106 [host down]
Nmap scan report for 192.168.1.107 [host down]
Nmap scan report for 192.168.1.108 [host down]
Nmap scan report for 192.168.1.109 [host down]
Nmap scan report for 192.168.1.110 [host down]
Nmap scan report for 192.168.1.111 [host down]
Nmap scan report for 192.168.1.112 [host down]
Nmap scan report for 192.168.1.113 [host down]
Nmap scan report for 192.168.1.114 [host down]
Nmap scan report for 192.168.1.115 [host down]
Nmap scan report for 192.168.1.116 [host down]
Nmap scan report for 192.168.1.117 [host down]
Nmap scan report for 192.168.1.118 [host down]
Nmap scan report for 192.168.1.119 [host down]
Nmap scan report for 192.168.1.120 [host down]
Nmap scan report for 192.168.1.121 [host down]
Nmap scan report for 192.168.1.122 [host down]
Nmap scan report for 192.168.1.123 [host down]
Nmap scan report for 192.168.1.124 [host down]
Nmap scan report for 192.168.1.125 [host down]
Nmap scan report for 192.168.1.126 [host down]
Nmap scan report for 192.168.1.127 [host down]
Nmap scan report for 192.168.1.128 [host down]
Nmap scan report for 192.168.1.129 [host down]
Nmap scan report for 192.168.1.130 [host down]
Nmap scan report for 192.168.1.131 [host down]
Nmap scan report for 192.168.1.132 [host down]
Nmap scan report for 192.168.1.133 [host down]
Nmap scan report for 192.168.1.134 [host down]
Nmap scan report for 192.168.1.135 [host down]
Nmap scan report for 192.168.1.136 [host down]
Nmap scan report for 192.168.1.137 [host down]
Nmap scan report for 192.168.1.138 [host down]
Nmap scan report for 192.168.1.139 [host down]
Nmap scan report for 192.168.1.140 [host down]
Nmap scan report for 192.168.1.141 [host down]
Nmap scan report for 192.168.1.142 [host down]
Nmap scan report for 192.168.1.143 [host down]
Nmap scan report for 192.168.1.144 [host down]
Nmap scan report for 192.168.1.145 [host down]
Nmap scan report for 192.168.1.146 [host down]
Nmap scan report for 192.168.1.147 [host down]
Nmap scan report for 192.168.1.148 [host down]
Nmap scan report for 192.168.1.149 [host down]
Nmap scan report for 192.168.1.150 [host down]
Nmap scan report for 192.168.1.151 [host down]
Nmap scan report for 192.168.1.152 [host down]
Nmap scan report for 192.168.1.153 [host down]
Nmap scan report for 192.168.1.154 [host down]
Nmap scan report for 192.168.1.155 [host down]
Nmap scan report for 192.168.1.156 [host down]
Nmap scan report for 192.168.1.157 [host down]
Nmap scan report for 192.168.1.158 [host down]
Nmap scan report for 192.168.1.159 [host down]
Nmap scan report for 192.168.1.160 [host down]
Nmap scan report for 192.168.1.161 [host down]
Nmap scan report for 192.168.1.162 [host down]
Nmap scan report for 192.168.1.163 [host down]
Nmap scan report for 192.168.1.164 [host down]
Nmap scan report for 192.168.1.165 [host down]
Nmap scan report for 192.168.1.166 [host down]
Nmap scan report for 192.168.1.167 [host down]
Nmap scan report for 192.168.1.168 [host down]
Nmap scan report for 192.168.1.169 [host down]
Nmap scan report for 192.168.1.170 [host down]
Nmap scan report for 192.168.1.171 [host down]
Nmap scan report for 192.168.1.172 [host down]
Nmap scan report for 192.168.1.173 [host down]
Nmap scan report for 192.168.1.174 [host down]
Nmap scan report for 192.168.1.175 [host down]
Nmap scan report for 192.168.1.176 [host down]
Nmap scan report for 192.168.1.177 [host down]
Nmap scan report for 192.168.1.178 [host down]
Nmap scan report for 192.168.1.179 [host down]
Nmap scan report for 192.168.1.180 [host down]
Nmap scan report for 192.168.1.181 [host down]
Nmap scan report for 192.168.1.182 [host down]
Nmap scan report for 192.168.1.183 [host down]
Nmap scan report for 192.168.1.184 [host down]
Nmap scan report for 192.168.1.185 [host down]
Nmap scan report for 192.168.1.186 [host down]
Nmap scan report for 192.168.1.187 [host down]
Nmap scan report for 192.168.1.188 [host down]
Nmap scan report for 192.168.1.189 [host down]
Nmap scan report for 192.168.1.190 [host down]
Nmap scan report for 192.168.1.191 [host down]
Nmap scan report for 192.168.1.192 [host down]
Nmap scan report for 192.168.1.193 [host down]
Nmap scan report for 192.168.1.194 [host down]
Nmap scan report for 192.168.1.195 [host down]
Nmap scan report for 192.168.1.196 [host down]
Nmap scan report for 192.168.1.197 [host down]
Nmap scan report for 192.168.1.198 [host down]
Nmap scan report for 192.168.1.199 [host down]
Nmap scan report for 192.168.1.200 [host down]
Nmap scan report for 192.168.1.201 [host down]
Nmap scan report for 192.168.1.202 [host down]
Nmap scan report for 192.168.1.203 [host down]
Nmap scan report for 192.168.1.204 [host down]
Nmap scan report for 192.168.1.205 [host down]
Nmap scan report for 192.168.1.206 [host down]
Nmap scan report for 192.168.1.207 [host down]
Nmap scan report for 192.168.1.208 [host down]
Nmap scan report for 192.168.1.209 [host down]
Nmap scan report for 192.168.1.210 [host down]
Nmap scan report for 192.168.1.211 [host down]
Nmap scan report for 192.168.1.212 [host down]
Nmap scan report for 192.168.1.213 [host down]
Nmap scan report for 192.168.1.214 [host down]
Nmap scan report for 192.168.1.215 [host down]
Nmap scan report for 192.168.1.216 [host down]
Nmap scan report for 192.168.1.217 [host down]
Nmap scan report for 192.168.1.218 [host down]
Nmap scan report for 192.168.1.219 [host down]
Nmap scan report for 192.168.1.220 [host down]
Nmap scan report for 192.168.1.221 [host down]
Nmap scan report for 192.168.1.222 [host down]
Nmap scan report for 192.168.1.223 [host down]
Nmap scan report for 192.168.1.224 [host down]
Nmap scan report for 192.168.1.225 [host down]
Nmap scan report for 192.168.1.226 [host down]
Nmap scan report for 192.168.1.227 [host down]
Nmap scan report for 192.168.1.228 [host down]
Nmap scan report for 192.168.1.229 [host down]
Nmap scan report for 192.168.1.230 [host down]
Nmap scan report for 192.168.1.231 [host down]
Nmap scan report for 192.168.1.232 [host down]
Nmap scan report for 192.168.1.233 [host down]
Nmap scan report for 192.168.1.234 [host down]
Nmap scan report for 192.168.1.235 [host down]
Nmap scan report for 192.168.1.236 [host down]
Nmap scan report for 192.168.1.237 [host down]
Nmap scan report for 192.168.1.238 [host down]
Nmap scan report for 192.168.1.239 [host down]
Nmap scan report for 192.168.1.240 [host down]
Nmap scan report for 192.168.1.241 [host down]
Nmap scan report for 192.168.1.242 [host down]
Nmap scan report for 192.168.1.243 [host down]
Nmap scan report for 192.168.1.244 [host down]
Nmap scan report for 192.168.1.245 [host down]
Nmap scan report for 192.168.1.246 [host down]
Nmap scan report for 192.168.1.247 [host down]
Nmap scan report for 192.168.1.248 [host down]
Nmap scan report for 192.168.1.249 [host down]
Nmap scan report for 192.168.1.250 [host down]
Nmap scan report for 192.168.1.251 [host down]
Nmap scan report for 192.168.1.252 [host down]
Nmap scan report for 192.168.1.253 [host down]
Nmap scan report for 192.168.1.254 [host down]
Initiating Parallel DNS resolution of 1 host. at 10:59
Completed Parallel DNS resolution of 1 host. at 10:59, 0.51s elapsed
Initiating SYN Stealth Scan at 10:59
Scanning 5 hosts [65535 ports/host]
RTTVAR has grown to over 2.3 seconds, decreasing to 2.0
RTTVAR has grown to over 2.3 seconds, decreasing to 2.0
Discovered open port 8080/tcp on 192.168.1.3
Discovered open port 80/tcp on 192.168.1.1
Discovered open port 443/tcp on 192.168.1.1
SYN Stealth Scan Timing: About 2.18% done; ETC: 11:23 (0:23:14 remaining)
SYN Stealth Scan Timing: About 3.71% done; ETC: 11:26 (0:26:23 remaining)
Increasing send delay for 192.168.1.4 from 0 to 5 due to max_successful_tryno increase to 5
SYN Stealth Scan Timing: About 8.70% done; ETC: 11:26 (0:24:51 remaining)
Discovered open port 15500/tcp on 192.168.1.3
Discovered open port 45061/tcp on 192.168.1.3
Discovered open port 9080/tcp on 192.168.1.3
Increasing send delay for 192.168.1.2 from 0 to 5 due to max_successful_tryno increase to 5
Discovered open port 9000/tcp on 192.168.1.5
Increasing send delay for 192.168.1.2 from 5 to 10 due to max_successful_tryno increase to 6
Discovered open port 6467/tcp on 192.168.1.5
SYN Stealth Scan Timing: About 18.75% done; ETC: 11:28 (0:23:29 remaining)
Discovered open port 45221/tcp on 192.168.1.3
Discovered open port 38231/tcp on 192.168.1.5
Discovered open port 38231/tcp on 192.168.1.5
SYN Stealth Scan Timing: About 22.74% done; ETC: 11:27 (0:21:58 remaining)
Increasing send delay for 192.168.1.4 from 5 to 10 due to max_successful_tryno increase to 6
SYN Stealth Scan Timing: About 26.68% done; ETC: 11:27 (0:20:31 remaining)
Discovered open port 7678/tcp on 192.168.1.3
Discovered open port 8008/tcp on 192.168.1.5
SYN Stealth Scan Timing: About 32.79% done; ETC: 11:27 (0:19:06 remaining)
Warning: 192.168.1.4 giving up on port because retransmission cap hit (6).
Discovered open port 8001/tcp on 192.168.1.3
SYN Stealth Scan Timing: About 38.68% done; ETC: 11:28 (0:17:37 remaining)
Discovered open port 40883/tcp on 192.168.1.5
Discovered open port 40883/tcp on 192.168.1.5
Discovered open port 10152/tcp on 192.168.1.4
SYN Stealth Scan Timing: About 45.22% done; ETC: 11:29 (0:16:08 remaining)
Warning: 192.168.1.2 giving up on port because retransmission cap hit (6).
Discovered open port 9197/tcp on 192.168.1.3
Discovered open port 8187/tcp on 192.168.1.3
Discovered open port 6466/tcp on 192.168.1.5
Discovered open port 6466/tcp on 192.168.1.5
Discovered open port 7000/tcp on 192.168.1.3
SYN Stealth Scan Timing: About 51.90% done; ETC: 11:30 (0:14:40 remaining)
Discovered open port 8002/tcp on 192.168.1.3
SYN Stealth Scan Timing: About 56.98% done; ETC: 11:29 (0:13:02 remaining)
Completed SYN Stealth Scan against 192.168.1.3 in 1038.02s (4 hosts left)
Discovered open port 8009/tcp on 192.168.1.5
SYN Stealth Scan Timing: About 61.87% done; ETC: 11:29 (0:11:28 remaining)
Discovered open port 38197/tcp on 192.168.1.5
Discovered open port 8443/tcp on 192.168.1.5
Discovered open port 6091/tcp on 192.168.1.5
Completed SYN Stealth Scan against 192.168.1.5 in 1130.94s (3 hosts left)
Discovered open port 37591/tcp on 192.168.1.1
SYN Stealth Scan Timing: About 73.15% done; ETC: 11:36 (0:09:57 remaining)
Discovered open port 46888/tcp on 192.168.1.4
SYN Stealth Scan Timing: About 80.18% done; ETC: 11:40 (0:08:05 remaining)
adjust_timeouts2: packet supposedly had rtt of 139494000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139494000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139479000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139479000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139526000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139526000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139393000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139393000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139467000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139467000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139506000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139506000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139419000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139419000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139369000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139369000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139526000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139526000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139509000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139509000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139481000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139481000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139493000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139493000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139392000 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of 139392000 microseconds.  Ignoring time.
SYN Stealth Scan Timing: About 86.89% done; ETC: 11:45 (0:06:02 remaining)
Completed SYN Stealth Scan against 192.168.1.2 in 2758.76s (2 hosts left)
SYN Stealth Scan Timing: About 89.16% done; ETC: 11:51 (0:05:36 remaining)
SYN Stealth Scan Timing: About 89.21% done; ETC: 11:57 (0:06:15 remaining)
Discovered open port 10150/tcp on 192.168.1.4
Completed SYN Stealth Scan against 192.168.1.4 in 3130.73s (1 host left)
SYN Stealth Scan Timing: About 94.51% done; ETC: 12:00 (0:03:20 remaining)
SYN Stealth Scan Timing: About 98.36% done; ETC: 12:01 (0:01:01 remaining)
Completed SYN Stealth Scan at 12:01, 3731.57s elapsed (327675 total ports)
Initiating Service scan at 12:01
Scanning 27 services on 5 hosts
WARNING: Service 192.168.1.1:80 had already soft-matched rtsp, but now soft-matched sip; ignoring second value
WARNING: Service 192.168.1.1:443 had already soft-matched rtsp, but now soft-matched sip; ignoring second value
Completed Service scan at 12:04, 164.76s elapsed (27 services on 5 hosts)
Initiating OS detection (try #1) against 5 hosts
Retrying OS detection (try #2) against 2 hosts
WARNING: OS didn't match until try #2
Retrying OS detection (try #3) against 192.168.1.5
Retrying OS detection (try #4) against 192.168.1.5
Retrying OS detection (try #5) against 192.168.1.5
NSE: Script scanning 5 hosts.
Initiating NSE at 12:04
Completed NSE at 12:05, 51.48s elapsed
Initiating NSE at 12:05
Completed NSE at 12:05, 8.07s elapsed
Initiating NSE at 12:05
Completed NSE at 12:05, 0.02s elapsed
Nmap scan report for dsldevice.lan (192.168.1.1)
Host is up (0.0051s latency).
Not shown: 65526 filtered tcp ports (no-response)
PORT      STATE  SERVICE      VERSION
80/tcp    open   rtsp
| fingerprint-strings: 
|   GetRequest: 
|     HTTP/1.0 200 OK
|     Cache-Control:private,max-age=0;
|     X-Frame-Options:SAMEORIGIN
|     X-Content-Type-Options:nosniff
|     X-XSS-Protection:1; mode=block
|     Content-Security-Policy:default-src 'self' blob: 'unsafe-inline' 'unsafe-eval';img-src * data: 'unsafe-inline'
|     Strict-Transport-Security:max-age=2592000; includeSubdomains
|     Referrer-Policy: no-referrer
|     Set-Cookie: lang=eng; path=/;
|     Content-type:text/html;charset=UTF-8;
|     &lt;!-- vim:fenc=utf-8
|     &lt;html&gt;
|     &lt;head&gt;
|     &lt;title&gt;
|     GPON Home Gateway
|     &lt;/title&gt; 
|     &lt;meta http-equiv="Content-Type" content="text/html; charset=UTF-8" /&gt;
|     &lt;meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/&gt;
|     &lt;meta name="referrer" content="no-referrer"/&gt;
|     &lt;script&gt;if(self!=top) top.location=self.location
|     if(!window.name){
|     location.reload();
|     window.name = 'Bell';
|     &lt;/script&gt;
|     &lt;link rel="stylesheet" href='/css_glb/main.css' type='text/css'/&gt;
|   HTTPOptions: 
|     HTTP/1.0 501 Not Implemented
|     Referrer-Policy: no-referrer
|     Server: thttpd
|     Content-Type: text/html; charset=utf-8
|     Date: Mon, 22 Sep 2025 06:31:54 GMT
|     Last-Modified: Mon, 22 Sep 2025 06:31:54 GMT
|     Accept-Ranges: bytes
|     Connection: close
|     Cache-Control: no-cache,no-store
|     &lt;HTML&gt;
|     &lt;HEAD&gt;&lt;TITLE&gt;501 Not Implemented&lt;/TITLE&gt;&lt;/HEAD&gt;
|     &lt;BODY BGCOLOR="#cc9999" TEXT="#000000" LINK="#2020ff" VLINK="#4040cc"&gt;
|     &lt;H2&gt;501 Not Implemented&lt;/H2&gt;
|     requested method 'OPTIONS' is not implemented by this server.
|     &lt;HR&gt;
|     &lt;/BODY&gt;
|     &lt;/HTML&gt;
|   RTSPRequest: 
|     RTSP/1.0 501 Not Implemented
|     Referrer-Policy: no-referrer
|     Server: thttpd
|     Content-Type: text/html; charset=utf-8
|     Date: Mon, 22 Sep 2025 06:31:54 GMT
|     Last-Modified: Mon, 22 Sep 2025 06:31:54 GMT
|     Accept-Ranges: bytes
|     Connection: close
|     Cache-Control: no-cache,no-store
|     &lt;HTML&gt;
|     &lt;HEAD&gt;&lt;TITLE&gt;501 Not Implemented&lt;/TITLE&gt;&lt;/HEAD&gt;
|     &lt;BODY BGCOLOR="#cc9999" TEXT="#000000" LINK="#2020ff" VLINK="#4040cc"&gt;
|     &lt;H2&gt;501 Not Implemented&lt;/H2&gt;
|     requested method 'OPTIONS' is not implemented by this server.
|     &lt;HR&gt;
|     &lt;/BODY&gt;
|_    &lt;/HTML&gt;
|_rtsp-methods: ERROR: Script execution failed (use -d to debug)
|_http-server-header: thttpd
443/tcp   open   ssl/rtsp
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.0 404 Not Found
|     Referrer-Policy: no-referrer
|     Server: thttpd
|     Content-Type: text/html; charset=utf-8
|     Date: Mon, 22 Sep 2025 06:32:01 GMT
|     Last-Modified: Mon, 22 Sep 2025 06:32:01 GMT
|     Accept-Ranges: bytes
|     Connection: close
|     Cache-Control: no-cache,no-store
|     &lt;html&gt;
|     &lt;head&gt;
|     &lt;/head&gt;
|     &lt;body&gt;
|     style="text-align: center; height: 150px"&gt;
|     &lt;span&gt;
|     Error 404 Not found
|     &lt;/span&gt;
|     &lt;/h1&gt;
|     style="text-align:center; font-size: 16px; font-weight: 400; padding: 10px 20px;"&gt;
|     requested URL was not found on this server
|     &lt;/p&gt;
|     &lt;div style="text-align: center;"&gt;
|     href="/"&gt;Home&lt;/a&gt;
|     &lt;/div&gt;
|     &lt;/body&gt;
|     &lt;/html&gt;
|     &lt;HR&gt;
|     &lt;/BODY&gt;
|     &lt;/HTML&gt;
|   GenericLines: 
|     UNKNOWN 400 Bad Request
|     Referrer-Policy: no-referrer
|     Server: thttpd
|     Content-Type: text/html; charset=utf-8
|     Date: Mon, 22 Sep 2025 06:32:07 GMT
|     Last-Modified: Mon, 22 Sep 2025 06:32:07 GMT
|     Accept-Ranges: bytes
|     Connection: close
|     Cache-Control: no-cache,no-store
|     &lt;HTML&gt;
|     &lt;HEAD&gt;&lt;TITLE&gt;400 Bad Request&lt;/TITLE&gt;&lt;/HEAD&gt;
|     &lt;BODY BGCOLOR="#cc9999" TEXT="#000000" LINK="#2020ff" VLINK="#4040cc"&gt;
|     &lt;H2&gt;400 Bad Request&lt;/H2&gt;
|     Your request has bad syntax or is inherently impossible to satisfy.
|     &lt;HR&gt;
|     &lt;/BODY&gt;
|     &lt;/HTML&gt;
|   RTSPRequest: 
|     RTSP/1.0 501 Not Implemented
|     Referrer-Policy: no-referrer
|     Server: thttpd
|     Content-Type: text/html; charset=utf-8
|     Date: Mon, 22 Sep 2025 06:32:07 GMT
|     Last-Modified: Mon, 22 Sep 2025 06:32:07 GMT
|     Accept-Ranges: bytes
|     Connection: close
|     Cache-Control: no-cache,no-store
|     &lt;HTML&gt;
|     &lt;HEAD&gt;&lt;TITLE&gt;501 Not Implemented&lt;/TITLE&gt;&lt;/HEAD&gt;
|     &lt;BODY BGCOLOR="#cc9999" TEXT="#000000" LINK="#2020ff" VLINK="#4040cc"&gt;
|     &lt;H2&gt;501 Not Implemented&lt;/H2&gt;
|     requested method 'OPTIONS' is not implemented by this server.
|     &lt;HR&gt;
|     &lt;/BODY&gt;
|_    &lt;/HTML&gt;
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=dsldevice.lan/organizationName=NSB/stateOrProvinceName=SH/countryName=CN
| Issuer: commonName=Nokia DHBU Root CA/organizationName=Nokia-DHBU/countryName=CN
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2016-09-07T06:17:48
| Not valid after:  2036-09-02T06:17:48
| MD5:     0a35 2b23 f76a f283 64d6 90a7 129e f181
| SHA-1:   3df4 7ec5 61d3 239a 7cb8 9544 e252 ad58 283e b176
|_SHA-256: 3638 08fa 22fc 15ac 26b8 3337 cf9b 6d2f a283 35bc 0053 69bd d9cc 0b74 a6c1 a40c
|_http-server-header: thttpd
445/tcp   closed microsoft-ds
8008/tcp  closed http
37591/tcp open   unknown
49156/tcp closed unknown
49157/tcp closed unknown
49160/tcp closed unknown
49161/tcp closed unknown
2 services unrecognized despite returning data. If you know the service/version, please submit the following fingerprints at https://nmap.org/cgi-bin/submit.cgi?new-service :
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port80-TCP:V=7.97%I=7%D=9/22%Time=68D0ED5A%P=i686-pc-windows-windows%r(
SF:GetRequest,2DB1,"HTTP/1\.0\x20200\x20OK\r\nCache-Control:private,max-ag
SF:e=0;\r\nX-Frame-Options:SAMEORIGIN\r\nX-Content-Type-Options:nosniff\r\
SF:nX-XSS-Protection:1;\x20mode=block\r\nContent-Security-Policy:default-s
SF:rc\x20'self'\x20blob:\x20'unsafe-inline'\x20'unsafe-eval';img-src\x20\*
SF:\x20data:\x20'unsafe-inline'\r\nStrict-Transport-Security:max-age=25920
SF:00;\x20includeSubdomains\r\nReferrer-Policy:\x20no-referrer\r\nSet-Cook
SF:ie:\x20lang=eng;\x20path=/;\r\nContent-type:text/html;charset=UTF-8;\r\
SF:n\r\n&lt;!--\x20vim:fenc=utf-8\r\n--&gt;\r\n&lt;html&gt;\r\n&lt;head&gt;\r\n&lt;title&gt;\r\n\r
SF:\nGPON\x20Home\x20Gateway\r\n\r\n&lt;/title&gt;\t\t\r\n&lt;meta\x20http-equiv=\"
SF:Content-Type\"\x20content=\"text/html;\x20charset=UTF-8\"\x20/&gt;\r\n&lt;met
SF:a\x20http-equiv=\"X-UA-Compatible\"\x20content=\"IE=edge,chrome=1\"/&gt;\r
SF:\n&lt;meta\x20name=\"referrer\"\x20content=\"no-referrer\"/&gt;\r\n&lt;script&gt;if
SF:\(self!=top\)\x20top\.location=self\.location\r\n\r\nif\(!window\.name\
SF:){\r\n\x20\x20\x20\x20\x20\x20\x20\x20location\.reload\(\);\r\n\x20\x20
SF:\x20\x20\x20\x20\x20\x20window\.name\x20=\x20'Bell';\r\n}\r\n&lt;/script&gt;\
SF:r\n&lt;link\x20rel=\"stylesheet\"\x20href='/css_glb/main\.css'\x20type='te
SF:xt/css'/&gt;\r\n&lt;")%r(HTTPOptions,206,"HTTP/1\.0\x20501\x20Not\x20Implemen
SF:ted\r\nReferrer-Policy:\x20no-referrer\r\nServer:\x20thttpd\r\nContent-
SF:Type:\x20text/html;\x20charset=utf-8\r\nDate:\x20Mon,\x2022\x20Sep\x202
SF:025\x2006:31:54\x20GMT\r\nLast-Modified:\x20Mon,\x2022\x20Sep\x202025\x
SF:2006:31:54\x20GMT\r\nAccept-Ranges:\x20bytes\r\nConnection:\x20close\r\
SF:nCache-Control:\x20no-cache,no-store\r\n\r\n&lt;HTML&gt;\n&lt;HEAD&gt;&lt;TITLE&gt;501\x2
SF:0Not\x20Implemented&lt;/TITLE&gt;&lt;/HEAD&gt;\n&lt;BODY\x20BGCOLOR=\"#cc9999\"\x20TEX
SF:T=\"#000000\"\x20LINK=\"#2020ff\"\x20VLINK=\"#4040cc\"&gt;\n&lt;H2&gt;501\x20Not
SF:\x20Implemented&lt;/H2&gt;\nThe\x20requested\x20method\x20'OPTIONS'\x20is\x20
SF:not\x20implemented\x20by\x20this\x20server\.\n&lt;HR&gt;\n&lt;/BODY&gt;\n&lt;/HTML&gt;\n"
SF:)%r(RTSPRequest,206,"RTSP/1\.0\x20501\x20Not\x20Implemented\r\nReferrer
SF:-Policy:\x20no-referrer\r\nServer:\x20thttpd\r\nContent-Type:\x20text/h
SF:tml;\x20charset=utf-8\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:31:54
SF:\x20GMT\r\nLast-Modified:\x20Mon,\x2022\x20Sep\x202025\x2006:31:54\x20G
SF:MT\r\nAccept-Ranges:\x20bytes\r\nConnection:\x20close\r\nCache-Control:
SF:\x20no-cache,no-store\r\n\r\n&lt;HTML&gt;\n&lt;HEAD&gt;&lt;TITLE&gt;501\x20Not\x20Impleme
SF:nted&lt;/TITLE&gt;&lt;/HEAD&gt;\n&lt;BODY\x20BGCOLOR=\"#cc9999\"\x20TEXT=\"#000000\"\x
SF:20LINK=\"#2020ff\"\x20VLINK=\"#4040cc\"&gt;\n&lt;H2&gt;501\x20Not\x20Implemented
SF:&lt;/H2&gt;\nThe\x20requested\x20method\x20'OPTIONS'\x20is\x20not\x20implemen
SF:ted\x20by\x20this\x20server\.\n&lt;HR&gt;\n&lt;/BODY&gt;\n&lt;/HTML&gt;\n");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port443-TCP:V=7.97%T=SSL%I=7%D=9/22%Time=68D0ED61%P=i686-pc-windows-win
SF:dows%r(FourOhFourRequest,292,"HTTP/1\.0\x20404\x20Not\x20Found\r\nRefer
SF:rer-Policy:\x20no-referrer\r\nServer:\x20thttpd\r\nContent-Type:\x20tex
SF:t/html;\x20charset=utf-8\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:32
SF::01\x20GMT\r\nLast-Modified:\x20Mon,\x2022\x20Sep\x202025\x2006:32:01\x
SF:20GMT\r\nAccept-Ranges:\x20bytes\r\nConnection:\x20close\r\nCache-Contr
SF:ol:\x20no-cache,no-store\r\n\r\n&lt;html&gt;\n&lt;head&gt;\n\n&lt;/head&gt;\n&lt;body&gt;\n\t&lt;h
SF:1\x20style=\"text-align:\x20center;\x20height:\x20150px\"&gt;\n\t\t&lt;span&gt;\
SF:n\t\t\tError\x20404\x20Not\x20found\n\t\t&lt;/span&gt;\n\x20\x20\x20\x20&lt;/h1&gt;
SF:\n\x20\x20\x20\x20&lt;p\x20style=\"text-align:center;\x20font-size:\x2016p
SF:x;\x20font-weight:\x20400;\x20padding:\x2010px\x2020px;\"&gt;\n\x20\x20\x2
SF:0\x20\x20\x20\x20\x20The\x20requested\x20URL\x20was\x20not\x20found\x20
SF:on\x20this\x20server\n\x20\x20\x20\x20\x20&lt;/p&gt;\n\t&lt;div\x20style=\"text-
SF:align:\x20center;\"&gt;\n\t\t&lt;a\x20href=\"/\"&gt;Home&lt;/a&gt;\n\t&lt;/div&gt;\n&lt;/body&gt;\
SF:n&lt;/html&gt;\n&lt;HR&gt;\n&lt;/BODY&gt;\n&lt;/HTML&gt;\n")%r(GenericLines,1FB,"UNKNOWN\x20400
SF:\x20Bad\x20Request\r\nReferrer-Policy:\x20no-referrer\r\nServer:\x20tht
SF:tpd\r\nContent-Type:\x20text/html;\x20charset=utf-8\r\nDate:\x20Mon,\x2
SF:022\x20Sep\x202025\x2006:32:07\x20GMT\r\nLast-Modified:\x20Mon,\x2022\x
SF:20Sep\x202025\x2006:32:07\x20GMT\r\nAccept-Ranges:\x20bytes\r\nConnecti
SF:on:\x20close\r\nCache-Control:\x20no-cache,no-store\r\n\r\n&lt;HTML&gt;\n&lt;HEA
SF:D&gt;&lt;TITLE&gt;400\x20Bad\x20Request&lt;/TITLE&gt;&lt;/HEAD&gt;\n&lt;BODY\x20BGCOLOR=\"#cc99
SF:99\"\x20TEXT=\"#000000\"\x20LINK=\"#2020ff\"\x20VLINK=\"#4040cc\"&gt;\n&lt;H2
SF:&gt;400\x20Bad\x20Request&lt;/H2&gt;\nYour\x20request\x20has\x20bad\x20syntax\x2
SF:0or\x20is\x20inherently\x20impossible\x20to\x20satisfy\.\n&lt;HR&gt;\n&lt;/BODY&gt;
SF:\n&lt;/HTML&gt;\n")%r(RTSPRequest,206,"RTSP/1\.0\x20501\x20Not\x20Implemented
SF:\r\nReferrer-Policy:\x20no-referrer\r\nServer:\x20thttpd\r\nContent-Typ
SF:e:\x20text/html;\x20charset=utf-8\r\nDate:\x20Mon,\x2022\x20Sep\x202025
SF:\x2006:32:07\x20GMT\r\nLast-Modified:\x20Mon,\x2022\x20Sep\x202025\x200
SF:6:32:07\x20GMT\r\nAccept-Ranges:\x20bytes\r\nConnection:\x20close\r\nCa
SF:che-Control:\x20no-cache,no-store\r\n\r\n&lt;HTML&gt;\n&lt;HEAD&gt;&lt;TITLE&gt;501\x20No
SF:t\x20Implemented&lt;/TITLE&gt;&lt;/HEAD&gt;\n&lt;BODY\x20BGCOLOR=\"#cc9999\"\x20TEXT=\
SF:"#000000\"\x20LINK=\"#2020ff\"\x20VLINK=\"#4040cc\"&gt;\n&lt;H2&gt;501\x20Not\x2
SF:0Implemented&lt;/H2&gt;\nThe\x20requested\x20method\x20'OPTIONS'\x20is\x20not
SF:\x20implemented\x20by\x20this\x20server\.\n&lt;HR&gt;\n&lt;/BODY&gt;\n&lt;/HTML&gt;\n");
MAC Address: 60:BD:2C:67:31:C0 (Taicang T&amp;W Electronics)
Device type: general purpose
Running: Linux 3.X|4.X
OS CPE: cpe:/o:linux:linux_kernel:3 cpe:/o:linux:linux_kernel:4
OS details: Linux 3.11 - 4.9
Uptime guess: 1.160 days (since Sun Sep 21 08:14:49 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=257 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT     ADDRESS
1   5.08 ms dsldevice.lan (192.168.1.1)

Nmap scan report for 192.168.1.2
Host is up (0.23s latency).
All 65535 scanned ports on 192.168.1.2 are in ignored states.
Not shown: 65468 closed tcp ports (reset), 67 filtered tcp ports (no-response)
MAC Address: 5A:08:F4:EF:5F:2E (Unknown)
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: general purpose|media device|specialized
Running: Microsoft Windows 10|11|2016, Microsoft Xbox 360, NTI embedded
OS CPE: cpe:/o:microsoft:windows_10 cpe:/o:microsoft:windows_11 cpe:/o:microsoft:windows_server_2016 cpe:/h:microsoft:xbox_360_kernel
OS details: Microsoft Windows 10 - 11, Microsoft Windows Server 2016, Microsoft Xbox 360 Dashboard, NTI E-MICRO-TRHP temperature sensor
Network Distance: 1 hop

TRACEROUTE
HOP RTT       ADDRESS
1   226.65 ms 192.168.1.2

Nmap scan report for 192.168.1.3
Host is up (0.0044s latency).
Not shown: 65524 closed tcp ports (reset)
PORT      STATE SERVICE             VERSION
7000/tcp  open  rtsp                AirTunes rtspd 377.40.00
|_rtsp-methods: ERROR: Script execution failed (use -d to debug)
|_irc-info: Unable to open connection
7678/tcp  open  upnp                Samsung AllShare upnpd 1.0 (UPnP 1.1)
8001/tcp  open  vcom-tunnel?
| fingerprint-strings: 
|   DNSStatusRequestTCP, DNSVersionBindReqTCP, Help, RPCCheck, SSLSessionReq: 
|     HTTP/1.0 403 Forbidden
|     content-type: text/html
|     content-length: 173
|     &lt;html&gt;&lt;head&gt;&lt;meta charset=utf-8 http-equiv="Content-Language" content="en"/&gt;&lt;link rel="stylesheet" type="text/css" href="/error.css"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;
|   FourOhFourRequest: 
|     HTTP/1.0 404 Not Found
|     content-type: application/json; charset=utf-8
|     content-length: 29
|     &lt;html&gt;&lt;body&gt;404&lt;/body&gt;&lt;/html&gt;
|   GetRequest: 
|     HTTP/1.0 401 Unauthorized
|     content-length: 29
|     &lt;html&gt;&lt;body&gt;401&lt;/body&gt;&lt;/html&gt;
|   HTTPOptions, RTSPRequest: 
|     HTTP/1.0 200 OK
|     content-type: application/json; charset=utf-8
|     access-control-allow-headers: content-type
|_    content-length: 3
8002/tcp  open  ssl/teradataordbms?
|_ssl-date: TLS randomness does not represent time
| fingerprint-strings: 
|   DNSStatusRequestTCP, DNSVersionBindReqTCP, Help, RPCCheck, SSLSessionReq: 
|     HTTP/1.0 403 Forbidden
|     content-type: text/html
|     content-length: 173
|     &lt;html&gt;&lt;head&gt;&lt;meta charset=utf-8 http-equiv="Content-Language" content="en"/&gt;&lt;link rel="stylesheet" type="text/css" href="/error.css"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;
|   GetRequest: 
|     HTTP/1.0 401 Unauthorized
|     content-length: 29
|     &lt;html&gt;&lt;body&gt;401&lt;/body&gt;&lt;/html&gt;
|   HTTPOptions, RTSPRequest: 
|     HTTP/1.0 200 OK
|     content-type: application/json; charset=utf-8
|     access-control-allow-headers: content-type
|_    content-length: 3
| ssl-cert: Subject: commonName=Samsung SmartViewSDK Cert. G2/organizationName=Samsung Electronics/countryName=KR
| Issuer: commonName=SmartViewSDK Root CA G2/organizationName=Samsung Electronics/countryName=KR
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha512WithRSAEncryption
| Not valid before: 2022-04-07T01:30:51
| Not valid after:  2072-03-25T01:30:51
| MD5:     e7c3 b159 e09d 4f73 a33c 4bcc 66d9 e540
| SHA-1:   c63e 4e59 d6c5 a4b0 3d3c e1b8 4a1b f191 31bd 72a2
|_SHA-256: 8fd9 7833 aeaf 0325 4ee9 3653 0e32 47b4 0b03 4684 b333 3dab f93e 2fd8 7631 fa48
| tls-alpn: 
|_  http/1.1
8080/tcp  open  http-proxy          WebServer
|_http-server-header: WebServer
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.0 404 Not Found
|     Content-Type: text/html
|     Access-Control-Allow-Origin: *
|     Access-Control-Allow-Headers: Content-Type
|     Content-Length: 341
|     Connection: close
|     Date: Mon, 22 Sep 2025 06:31:50 GMT
|     Server: WebServer
|     &lt;?xml version="1.0" encoding="iso-8859-1"?&gt;
|     &lt;!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
|     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"&gt;
|     &lt;html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"&gt;
|     &lt;head&gt;
|     &lt;title&gt;404 Not Found&lt;/title&gt;
|     &lt;/head&gt;
|     &lt;body&gt;
|     &lt;h1&gt;404 Not Found&lt;/h1&gt;
|     &lt;/body&gt;
|     &lt;/html&gt;
|   GetRequest: 
|     HTTP/1.0 403 Forbidden
|     Content-Type: text/html
|     Access-Control-Allow-Origin: *
|     Access-Control-Allow-Headers: Content-Type
|     Content-Length: 341
|     Connection: close
|     Date: Mon, 22 Sep 2025 06:31:49 GMT
|     Server: WebServer
|     &lt;?xml version="1.0" encoding="iso-8859-1"?&gt;
|     &lt;!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
|     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"&gt;
|     &lt;html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"&gt;
|     &lt;head&gt;
|     &lt;title&gt;403 Forbidden&lt;/title&gt;
|     &lt;/head&gt;
|     &lt;body&gt;
|     &lt;h1&gt;403 Forbidden&lt;/h1&gt;
|     &lt;/body&gt;
|     &lt;/html&gt;
|   HTTPOptions: 
|     HTTP/1.0 200 OK
|     Allow: OPTIONS, GET, HEAD, POST
|     Access-Control-Allow-Origin: *
|     Access-Control-Allow-Headers: Content-Type
|     Content-Length: 0
|     Connection: close
|     Date: Mon, 22 Sep 2025 06:31:50 GMT
|     Server: WebServer
|   RTSPRequest: 
|     HTTP/1.0 400 Bad Request
|     Content-Type: text/html
|     Content-Length: 345
|     Connection: close
|     Date: Mon, 22 Sep 2025 06:31:50 GMT
|     Server: WebServer
|     &lt;?xml version="1.0" encoding="iso-8859-1"?&gt;
|     &lt;!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
|     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"&gt;
|     &lt;html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"&gt;
|     &lt;head&gt;
|     &lt;title&gt;400 Bad Request&lt;/title&gt;
|     &lt;/head&gt;
|     &lt;body&gt;
|     &lt;h1&gt;400 Bad Request&lt;/h1&gt;
|     &lt;/body&gt;
|_    &lt;/html&gt;
|_http-title: 403 Forbidden
| http-methods: 
|_  Supported Methods: OPTIONS GET HEAD POST
8187/tcp  open  upnp                Samsung AllShare upnpd 1.0 (UPnP 1.1)
9080/tcp  open  glrpc?
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.0 200 OK
|     Date: Mon, 22 Sep 2025 12:02:35 IST
|     Server: NRDP/2023.1.5.0-223bdfbfde9
|     Connection: close
|     Cache-Control: no-cache
|     Content-Length: 9
|     status=ok
|   GetRequest: 
|     HTTP/1.0 200 OK
|     Date: Mon, 22 Sep 2025 12:01:50 IST
|     Server: NRDP/2023.1.5.0-223bdfbfde9
|     Connection: close
|     Cache-Control: no-cache
|     Content-Length: 9
|_    status=ok
9197/tcp  open  upnp                Samsung AllShare upnpd 1.0 (UPnP 1.1)
15500/tcp open  unknown
45061/tcp open  unknown
| fingerprint-strings: 
|   FourOhFourRequest, GetRequest, HTTPOptions: 
|     HTTP/1.0 404 Not Found
|     Content-Length: 0
|_    Content-Type: text/plain
45221/tcp open  tcpwrapped
5 services unrecognized despite returning data. If you know the service/version, please submit the following fingerprints at https://nmap.org/cgi-bin/submit.cgi?new-service :
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port8001-TCP:V=7.97%I=7%D=9/22%Time=68D0ED57%P=i686-pc-windows-windows%
SF:r(GetRequest,4E,"HTTP/1\.0\x20401\x20Unauthorized\r\ncontent-length:\x2
SF:029\r\n\r\n&lt;html&gt;&lt;body&gt;401&lt;/body&gt;&lt;/html&gt;")%r(FourOhFourRequest,7A,"HTTP
SF:/1\.0\x20404\x20Not\x20Found\r\ncontent-type:\x20application/json;\x20c
SF:harset=utf-8\r\ncontent-length:\x2029\r\n\r\n&lt;html&gt;&lt;body&gt;404&lt;/body&gt;&lt;/ht
SF:ml&gt;")%r(HTTPOptions,84,"HTTP/1\.0\x20200\x20OK\r\ncontent-type:\x20appl
SF:ication/json;\x20charset=utf-8\r\naccess-control-allow-headers:\x20cont
SF:ent-type\r\ncontent-length:\x203\r\n\r\n200")%r(RTSPRequest,84,"HTTP/1\
SF:.0\x20200\x20OK\r\ncontent-type:\x20application/json;\x20charset=utf-8\
SF:r\naccess-control-allow-headers:\x20content-type\r\ncontent-length:\x20
SF:3\r\n\r\n200")%r(RPCCheck,F5,"HTTP/1\.0\x20403\x20Forbidden\r\ncontent-
SF:type:\x20text/html\r\ncontent-length:\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;&lt;meta\x
SF:20charset=utf-8\x20http-equiv=\"Content-Language\"\x20content=\"en\"/&gt;&lt;
SF:link\x20rel=\"stylesheet\"\x20type=\"text/css\"\x20href=\"/error\.css\"
SF:/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;")%r(DNSVersionBindReqTCP,F5,"
SF:HTTP/1\.0\x20403\x20Forbidden\r\ncontent-type:\x20text/html\r\ncontent-
SF:length:\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;&lt;meta\x20charset=utf-8\x20http-equiv=
SF:\"Content-Language\"\x20content=\"en\"/&gt;&lt;link\x20rel=\"stylesheet\"\x20
SF:type=\"text/css\"\x20href=\"/error\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/b
SF:ody&gt;&lt;/html&gt;")%r(DNSStatusRequestTCP,F5,"HTTP/1\.0\x20403\x20Forbidden\r
SF:\ncontent-type:\x20text/html\r\ncontent-length:\x20173\r\n\r\n&lt;html&gt;&lt;he
SF:ad&gt;&lt;meta\x20charset=utf-8\x20http-equiv=\"Content-Language\"\x20content
SF:=\"en\"/&gt;&lt;link\x20rel=\"stylesheet\"\x20type=\"text/css\"\x20href=\"/er
SF:ror\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;")%r(Help,F5,"HTTP/1
SF:\.0\x20403\x20Forbidden\r\ncontent-type:\x20text/html\r\ncontent-length
SF::\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;&lt;meta\x20charset=utf-8\x20http-equiv=\"Cont
SF:ent-Language\"\x20content=\"en\"/&gt;&lt;link\x20rel=\"stylesheet\"\x20type=\
SF:"text/css\"\x20href=\"/error\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/
SF:html&gt;")%r(SSLSessionReq,F5,"HTTP/1\.0\x20403\x20Forbidden\r\ncontent-ty
SF:pe:\x20text/html\r\ncontent-length:\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;&lt;meta\x20
SF:charset=utf-8\x20http-equiv=\"Content-Language\"\x20content=\"en\"/&gt;&lt;li
SF:nk\x20rel=\"stylesheet\"\x20type=\"text/css\"\x20href=\"/error\.css\"/&gt;
SF:&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port8002-TCP:V=7.97%T=SSL%I=7%D=9/22%Time=68D0ED62%P=i686-pc-windows-wi
SF:ndows%r(GetRequest,4E,"HTTP/1\.0\x20401\x20Unauthorized\r\ncontent-leng
SF:th:\x2029\r\n\r\n&lt;html&gt;&lt;body&gt;401&lt;/body&gt;&lt;/html&gt;")%r(HTTPOptions,84,"HTTP
SF:/1\.0\x20200\x20OK\r\ncontent-type:\x20application/json;\x20charset=utf
SF:-8\r\naccess-control-allow-headers:\x20content-type\r\ncontent-length:\
SF:x203\r\n\r\n200")%r(RTSPRequest,84,"HTTP/1\.0\x20200\x20OK\r\ncontent-t
SF:ype:\x20application/json;\x20charset=utf-8\r\naccess-control-allow-head
SF:ers:\x20content-type\r\ncontent-length:\x203\r\n\r\n200")%r(RPCCheck,F5
SF:,"HTTP/1\.0\x20403\x20Forbidden\r\ncontent-type:\x20text/html\r\nconten
SF:t-length:\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;&lt;meta\x20charset=utf-8\x20http-equi
SF:v=\"Content-Language\"\x20content=\"en\"/&gt;&lt;link\x20rel=\"stylesheet\"\x
SF:20type=\"text/css\"\x20href=\"/error\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;
SF:/body&gt;&lt;/html&gt;")%r(DNSVersionBindReqTCP,F5,"HTTP/1\.0\x20403\x20Forbidde
SF:n\r\ncontent-type:\x20text/html\r\ncontent-length:\x20173\r\n\r\n&lt;html&gt;
SF:&lt;head&gt;&lt;meta\x20charset=utf-8\x20http-equiv=\"Content-Language\"\x20cont
SF:ent=\"en\"/&gt;&lt;link\x20rel=\"stylesheet\"\x20type=\"text/css\"\x20href=\"
SF:/error\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;")%r(DNSStatusReq
SF:uestTCP,F5,"HTTP/1\.0\x20403\x20Forbidden\r\ncontent-type:\x20text/html
SF:\r\ncontent-length:\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;&lt;meta\x20charset=utf-8\x2
SF:0http-equiv=\"Content-Language\"\x20content=\"en\"/&gt;&lt;link\x20rel=\"styl
SF:esheet\"\x20type=\"text/css\"\x20href=\"/error\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1
SF:&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;")%r(Help,F5,"HTTP/1\.0\x20403\x20Forbidden\r\nc
SF:ontent-type:\x20text/html\r\ncontent-length:\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;
SF:&lt;meta\x20charset=utf-8\x20http-equiv=\"Content-Language\"\x20content=\"
SF:en\"/&gt;&lt;link\x20rel=\"stylesheet\"\x20type=\"text/css\"\x20href=\"/error
SF:\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/body&gt;&lt;/html&gt;")%r(SSLSessionReq,F5,"
SF:HTTP/1\.0\x20403\x20Forbidden\r\ncontent-type:\x20text/html\r\ncontent-
SF:length:\x20173\r\n\r\n&lt;html&gt;&lt;head&gt;&lt;meta\x20charset=utf-8\x20http-equiv=
SF:\"Content-Language\"\x20content=\"en\"/&gt;&lt;link\x20rel=\"stylesheet\"\x20
SF:type=\"text/css\"\x20href=\"/error\.css\"/&gt;&lt;/head&gt;&lt;body&gt;&lt;h1&gt;403&lt;/h1&gt;&lt;/b
SF:ody&gt;&lt;/html&gt;");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port8080-TCP:V=7.97%I=7%D=9/22%Time=68D0ED57%P=i686-pc-windows-windows%
SF:r(GetRequest,234,"HTTP/1\.0\x20403\x20Forbidden\r\nContent-Type:\x20tex
SF:t/html\r\nAccess-Control-Allow-Origin:\x20\*\r\nAccess-Control-Allow-He
SF:aders:\x20Content-Type\r\nContent-Length:\x20341\r\nConnection:\x20clos
SF:e\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:31:49\x20GMT\r\nServer:\x
SF:20WebServer\r\n\r\n&lt;\?xml\x20version=\"1\.0\"\x20encoding=\"iso-8859-1\
SF:"\?&gt;\n&lt;!DOCTYPE\x20html\x20PUBLIC\x20\"-//W3C//DTD\x20XHTML\x201\.0\x20
SF:Transitional//EN\"\n\x20\x20\x20\x20\x20\x20\x20\x20\x20\"http://www\.w
SF:3\.org/TR/xhtml1/DTD/xhtml1-transitional\.dtd\"&gt;\n&lt;html\x20xmlns=\"http
SF:://www\.w3\.org/1999/xhtml\"\x20xml:lang=\"en\"\x20lang=\"en\"&gt;\n\x20&lt;h
SF:ead&gt;\n\x20\x20&lt;title&gt;403\x20Forbidden&lt;/title&gt;\n\x20&lt;/head&gt;\n\x20&lt;body&gt;\
SF:n\x20\x20&lt;h1&gt;403\x20Forbidden&lt;/h1&gt;\n\x20&lt;/body&gt;\n&lt;/html&gt;\n")%r(HTTPOpti
SF:ons,DE,"HTTP/1\.0\x20200\x20OK\r\nAllow:\x20OPTIONS,\x20GET,\x20HEAD,\x
SF:20POST\r\nAccess-Control-Allow-Origin:\x20\*\r\nAccess-Control-Allow-He
SF:aders:\x20Content-Type\r\nContent-Length:\x200\r\nConnection:\x20close\
SF:r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:31:50\x20GMT\r\nServer:\x20
SF:WebServer\r\n\r\n")%r(RTSPRequest,1EE,"HTTP/1\.0\x20400\x20Bad\x20Reque
SF:st\r\nContent-Type:\x20text/html\r\nContent-Length:\x20345\r\nConnectio
SF:n:\x20close\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:31:50\x20GMT\r\
SF:nServer:\x20WebServer\r\n\r\n&lt;\?xml\x20version=\"1\.0\"\x20encoding=\"i
SF:so-8859-1\"\?&gt;\n&lt;!DOCTYPE\x20html\x20PUBLIC\x20\"-//W3C//DTD\x20XHTML\x
SF:201\.0\x20Transitional//EN\"\n\x20\x20\x20\x20\x20\x20\x20\x20\x20\"htt
SF:p://www\.w3\.org/TR/xhtml1/DTD/xhtml1-transitional\.dtd\"&gt;\n&lt;html\x20xm
SF:lns=\"http://www\.w3\.org/1999/xhtml\"\x20xml:lang=\"en\"\x20lang=\"en\
SF:"&gt;\n\x20&lt;head&gt;\n\x20\x20&lt;title&gt;400\x20Bad\x20Request&lt;/title&gt;\n\x20&lt;/hea
SF:d&gt;\n\x20&lt;body&gt;\n\x20\x20&lt;h1&gt;400\x20Bad\x20Request&lt;/h1&gt;\n\x20&lt;/body&gt;\n&lt;/
SF:html&gt;\n")%r(FourOhFourRequest,234,"HTTP/1\.0\x20404\x20Not\x20Found\r\n
SF:Content-Type:\x20text/html\r\nAccess-Control-Allow-Origin:\x20\*\r\nAcc
SF:ess-Control-Allow-Headers:\x20Content-Type\r\nContent-Length:\x20341\r\
SF:nConnection:\x20close\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:31:50
SF:\x20GMT\r\nServer:\x20WebServer\r\n\r\n&lt;\?xml\x20version=\"1\.0\"\x20en
SF:coding=\"iso-8859-1\"\?&gt;\n&lt;!DOCTYPE\x20html\x20PUBLIC\x20\"-//W3C//DTD\
SF:x20XHTML\x201\.0\x20Transitional//EN\"\n\x20\x20\x20\x20\x20\x20\x20\x2
SF:0\x20\"http://www\.w3\.org/TR/xhtml1/DTD/xhtml1-transitional\.dtd\"&gt;\n&lt;
SF:html\x20xmlns=\"http://www\.w3\.org/1999/xhtml\"\x20xml:lang=\"en\"\x20
SF:lang=\"en\"&gt;\n\x20&lt;head&gt;\n\x20\x20&lt;title&gt;404\x20Not\x20Found&lt;/title&gt;\n\
SF:x20&lt;/head&gt;\n\x20&lt;body&gt;\n\x20\x20&lt;h1&gt;404\x20Not\x20Found&lt;/h1&gt;\n\x20&lt;/bod
SF:y&gt;\n&lt;/html&gt;\n");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port9080-TCP:V=7.97%I=7%D=9/22%Time=68D0ED57%P=i686-pc-windows-windows%
SF:r(GetRequest,A5,"HTTP/1\.0\x20200\x20OK\r\nDate:\x20Mon,\x2022\x20Sep\x
SF:202025\x2012:01:50\x20IST\r\nServer:\x20NRDP/2023\.1\.5\.0-223bdfbfde9\
SF:r\nConnection:\x20close\r\nCache-Control:\x20no-cache\r\nContent-Length
SF::\x209\r\n\r\nstatus=ok")%r(FourOhFourRequest,A5,"HTTP/1\.0\x20200\x20O
SF:K\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2012:02:35\x20IST\r\nServer:\x
SF:20NRDP/2023\.1\.5\.0-223bdfbfde9\r\nConnection:\x20close\r\nCache-Contr
SF:ol:\x20no-cache\r\nContent-Length:\x209\r\n\r\nstatus=ok");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port45061-TCP:V=7.97%I=7%D=9/22%Time=68D0ED5C%P=i686-pc-windows-windows
SF:%r(GetRequest,47,"HTTP/1\.0\x20404\x20Not\x20Found\r\nContent-Length:\x
SF:200\r\nContent-Type:\x20text/plain\r\n\r\n")%r(HTTPOptions,47,"HTTP/1\.
SF:0\x20404\x20Not\x20Found\r\nContent-Length:\x200\r\nContent-Type:\x20te
SF:xt/plain\r\n\r\n")%r(FourOhFourRequest,47,"HTTP/1\.0\x20404\x20Not\x20F
SF:ound\r\nContent-Length:\x200\r\nContent-Type:\x20text/plain\r\n\r\n");
MAC Address: 68:FC:CA:E6:97:04 (Samsung Electronics)
Device type: general purpose
Running: Linux 4.X|5.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5
OS details: Linux 4.15 - 5.19
Uptime guess: 17.119 days (since Fri Sep  5 09:14:33 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=249 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT     ADDRESS
1   4.40 ms 192.168.1.3

Nmap scan report for 192.168.1.4
Host is up (0.088s latency).
Not shown: 65507 closed tcp ports (reset)
PORT      STATE    SERVICE    VERSION
7/tcp     filtered echo
650/tcp   filtered obex
2101/tcp  filtered rtcm-sc104
3092/tcp  filtered unknown
9894/tcp  filtered unknown
10150/tcp open     unknown
10152/tcp open     unknown
15075/tcp filtered unknown
17737/tcp filtered unknown
19663/tcp filtered unknown
26127/tcp filtered unknown
28995/tcp filtered unknown
31937/tcp filtered unknown
34409/tcp filtered unknown
35374/tcp filtered unknown
39399/tcp filtered unknown
41413/tcp filtered unknown
44352/tcp filtered unknown
44797/tcp filtered unknown
46627/tcp filtered unknown
46888/tcp open     unknown
| fingerprint-strings: 
|   DNSStatusRequestTCP, DNSVersionBindReqTCP, GenericLines, GetRequest, HTTPOptions, Help, NULL, RPCCheck, RTSPRequest: 
|     OAFP_B22A6AE4B25CA41FCD63B12AE618A37 
|     CPH2625
|     OPPO
|_    OPPO Reno12 5G
48045/tcp filtered unknown
48623/tcp filtered unknown
53236/tcp filtered unknown
54902/tcp filtered unknown
58549/tcp filtered unknown
60827/tcp filtered unknown
65411/tcp filtered unknown
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port46888-TCP:V=7.97%I=7%D=9/22%Time=68D0ED57%P=i686-pc-windows-windows
SF:%r(NULL,6C,"\0j\x01\0\nOAFP_B22A6AE4B25CA41FCD63B12AE618A37\x20\r\x01\0
SF:\x10\0\0\x02\xff\xf5\x03\x03\xfe\x04'\x10\x05\0\n\x06\x07CPH2625\x07\x0
SF:4OPPO\x08\x0eOPPO\x20Reno12\x205G\n\x08\x0b\x01\x0c0\r\x01\x0e\x03\0\0\
SF:0\0\0\0\0")%r(GenericLines,6C,"\0j\x01\0\nOAFP_B22A6AE4B25CA41FCD63B12A
SF:E618A37\x20\r\x01\0\x10\0\0\x02\xff\xf5\x03\x03\xfe\x04'\x10\x05\0\n\x0
SF:6\x07CPH2625\x07\x04OPPO\x08\x0eOPPO\x20Reno12\x205G\n\x08\x0b\x01\x0c0
SF:\r\x01\x0e\x03\0\0\0\0\0\0\0")%r(GetRequest,6C,"\0j\x01\0\nOAFP_B22A6AE
SF:4B25CA41FCD63B12AE618A37\x20\r\x01\0\x10\0\0\x02\xff\xf5\x03\x03\xfe\x0
SF:4'\x10\x05\0\n\x06\x07CPH2625\x07\x04OPPO\x08\x0eOPPO\x20Reno12\x205G\n
SF:\x08\x0b\x01\x0c0\r\x01\x0e\x03\0\0\0\0\0\0\0")%r(HTTPOptions,6C,"\0j\x
SF:01\0\nOAFP_B22A6AE4B25CA41FCD63B12AE618A37\x20\r\x01\0\x10\0\0\x02\xff\
SF:xf5\x03\x03\xfe\x04'\x10\x05\0\n\x06\x07CPH2625\x07\x04OPPO\x08\x0eOPPO
SF:\x20Reno12\x205G\n\x08\x0b\x01\x0c0\r\x01\x0e\x03\0\0\0\0\0\0\0")%r(RTS
SF:PRequest,6C,"\0j\x01\0\nOAFP_B22A6AE4B25CA41FCD63B12AE618A37\x20\r\x01\
SF:0\x10\0\0\x02\xff\xf5\x03\x03\xfe\x04'\x10\x05\0\n\x06\x07CPH2625\x07\x
SF:04OPPO\x08\x0eOPPO\x20Reno12\x205G\n\x08\x0b\x01\x0c0\r\x01\x0e\x03\0\0
SF:\0\0\0\0\0")%r(RPCCheck,6C,"\0j\x01\0\nOAFP_B22A6AE4B25CA41FCD63B12AE61
SF:8A37\x20\r\x01\0\x10\0\0\x02\xff\xf5\x03\x03\xfe\x04'\x10\x05\0\n\x06\x
SF:07CPH2625\x07\x04OPPO\x08\x0eOPPO\x20Reno12\x205G\n\x08\x0b\x01\x0c0\r\
SF:x01\x0e\x03\0\0\0\0\0\0\0")%r(DNSVersionBindReqTCP,6C,"\0j\x01\0\nOAFP_
SF:B22A6AE4B25CA41FCD63B12AE618A37\x20\r\x01\0\x10\0\0\x02\xff\xf5\x03\x03
SF:\xfe\x04'\x10\x05\0\n\x06\x07CPH2625\x07\x04OPPO\x08\x0eOPPO\x20Reno12\
SF:x205G\n\x08\x0b\x01\x0c0\r\x01\x0e\x03\0\0\0\0\0\0\0")%r(DNSStatusReque
SF:stTCP,6C,"\0j\x01\0\nOAFP_B22A6AE4B25CA41FCD63B12AE618A37\x20\r\x01\0\x
SF:10\0\0\x02\xff\xf5\x03\x03\xfe\x04'\x10\x05\0\n\x06\x07CPH2625\x07\x04O
SF:PPO\x08\x0eOPPO\x20Reno12\x205G\n\x08\x0b\x01\x0c0\r\x01\x0e\x03\0\0\0\
SF:0\0\0\0")%r(Help,6C,"\0j\x01\0\nOAFP_B22A6AE4B25CA41FCD63B12AE618A37\x2
SF:0\r\x01\0\x10\0\0\x02\xff\xf5\x03\x03\xfe\x04'\x10\x05\0\n\x06\x07CPH26
SF:25\x07\x04OPPO\x08\x0eOPPO\x20Reno12\x205G\n\x08\x0b\x01\x0c0\r\x01\x0e
SF:\x03\0\0\0\0\0\0\0");
MAC Address: 26:43:1D:FE:39:5C (Unknown)
Device type: phone
Running: Linux 4.X, Google Android 10.X|11.X|12.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:google:android:10 cpe:/o:google:android:11 cpe:/o:google:android:12
OS details: Android 10 - 12 (Linux 4.14 - 4.19)
Uptime guess: 42.823 days (since Sun Aug 10 16:20:14 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=259 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT      ADDRESS
1   88.23 ms 192.168.1.4

Nmap scan report for 192.168.1.5
Host is up (0.061s latency).
Not shown: 65525 closed tcp ports (reset)
PORT      STATE SERVICE         VERSION
6091/tcp  open  unknown
6466/tcp  open  ssl/unknown
| ssl-cert: Subject: commonName=atvremote/rango/rango/MiTV-AXFR0/78:F2:35:34:00:6F
| Issuer: commonName=atvremote/rango/rango/MiTV-AXFR0/78:F2:35:34:00:6F
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2021-09-21T12:00:00
| Not valid after:  2038-01-19T03:14:07
| MD5:     dc6c 5bc3 aaf0 36fa de9c 5d24 d1c5 61c1
| SHA-1:   9630 b21f 4854 2c6c 2cb9 7f85 b484 d2c3 f590 0996
|_SHA-256: 2740 ab00 cd95 d32d dd95 e8c1 120e 457f 503b a4b6 2b24 ea9e a400 5f75 9e73 8341
|_ssl-date: TLS randomness does not represent time
6467/tcp  open  ssl/unknown
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=atvremote/rango/rango/MiTV-AXFR0/78:F2:35:34:00:6F
| Issuer: commonName=atvremote/rango/rango/MiTV-AXFR0/78:F2:35:34:00:6F
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2021-09-21T12:00:00
| Not valid after:  2038-01-19T03:14:07
| MD5:     dc6c 5bc3 aaf0 36fa de9c 5d24 d1c5 61c1
| SHA-1:   9630 b21f 4854 2c6c 2cb9 7f85 b484 d2c3 f590 0996
|_SHA-256: 2740 ab00 cd95 d32d dd95 e8c1 120e 457f 503b a4b6 2b24 ea9e a400 5f75 9e73 8341
8008/tcp  open  http?
|_http-title: Site doesn't have a title (text/html).
8009/tcp  open  ssl/castv2      Ninja Sphere Chromecast driver
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=9585064a-a783-7db7-3797-a75aa5f22d06
| Issuer: commonName=9585064a-a783-7db7-3797-a75aa5f22d06
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2025-09-21T18:15:07
| Not valid after:  2025-09-23T18:15:07
| MD5:     757a dff4 233e b181 ca8e c27d d588 de92
| SHA-1:   e307 0f1c 1ecc 38b2 a3aa e14b ef38 8d7e 2b73 d6d2
|_SHA-256: 8404 32b9 a558 1ef7 8654 d976 e2ca 0c3f 4a7e b681 b671 8812 3c6e 4a53 5fff 662f
|_ajp-methods: Failed to get a valid response for the OPTION request
8443/tcp  open  ssl/https-alt?
| ssl-cert: Subject: commonName=-7218888138564098524/organizationName=Google Inc/stateOrProvinceName=Washington/countryName=US
| Issuer: commonName=Xiaomi TV rango Amlogic AMLT950X4 Cast ICA/organizationName=Google Inc/stateOrProvinceName=Washington/countryName=US
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2021-11-05T11:17:51
| Not valid after:  2041-11-05T11:17:51
| MD5:     c3c3 5b1a 5e90 8fba eac7 3be9 da55 6825
| SHA-1:   9807 fae5 1bf7 dfcd 5cee 93bf 62ab dc4e 96e0 fb5b
|_SHA-256: e51c de6b 5078 6d10 1d50 680a 0941 6866 1a29 bde6 aede 3bf8 c00e bb79 ed0b 85f2
|_http-title: Site doesn't have a title (text/html).
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
9000/tcp  open  ssl/cslistener?
38197/tcp open  tcpwrapped
38231/tcp open  tcpwrapped
40883/tcp open  tcpwrapped
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port6091-TCP:V=7.97%I=7%D=9/22%Time=68D0ED57%P=i686-pc-windows-windows%
SF:r(NULL,6,"\x02\0\0\x02\0\0")%r(GenericLines,6,"\x02\0\0\x02\0\0")%r(Get
SF:Request,3,"\x02\0\0")%r(RPCCheck,3,"\x02\0\0")%r(DNSVersionBindReqTCP,3
SF:,"\x02\0\0")%r(Help,6,"\x02\0\0\x02\0\0")%r(SSLSessionReq,3,"\x02\0\0")
SF:%r(TerminalServerCookie,3,"\x02\0\0")%r(TLSSessionReq,3,"\x02\0\0")%r(K
SF:erberos,3,"\x02\0\0")%r(SMBProgNeg,3,"\x02\0\0")%r(X11Probe,3,"\x02\0\0
SF:")%r(LDAPSearchReq,3,"\x02\0\0")%r(LDAPBindReq,3,"\x02\0\0")%r(LANDesk-
SF:RC,3,"\x02\0\0")%r(NotesRPC,3,"\x02\0\0")%r(JavaRMI,3,"\x02\0\0")%r(ora
SF:cle-tns,3,"\x02\0\0")%r(ms-sql-s,3,"\x02\0\0")%r(afp,3,"\x02\0\0")%r(gi
SF:op,3,"\x02\0\0");
MAC Address: 3A:C0:1F:FA:EE:3A (Unknown)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.97%E=4%D=9/22%OT=6091%CT=1%CU=39349%PV=Y%DS=1%DC=D%G=Y%M=3AC01F
OS:%TM=68D0EE42%P=i686-pc-windows-windows)SEQ(SP=105%GCD=1%ISR=10B%TI=Z%CI=
OS:Z%II=I%TS=A)SEQ(SP=106%GCD=1%ISR=109%TI=Z%CI=Z%II=I%TS=A)SEQ(SP=107%GCD=
OS:1%ISR=10A%TI=Z%CI=Z%II=I%TS=A)SEQ(SP=109%GCD=1%ISR=107%TI=Z%CI=Z%II=I%TS
OS:=A)SEQ(SP=FD%GCD=1%ISR=10E%TI=Z%CI=Z%II=I%TS=A)OPS(O1=M5B4ST11NW7%O2=M5B
OS:4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7%O5=M5B4ST11NW7%O6=M5B4ST11)WIN(W
OS:1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=FFFF)ECN(R=Y%DF=Y%T=40%W=FFFF%
OS:O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=
OS:N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A
OS:=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%D
OS:F=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL
OS:=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=N%T=40%CD=S)

Uptime guess: 23.678 days (since Fri Aug 29 19:49:45 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=253 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT      ADDRESS
1   61.36 ms 192.168.1.5

Initiating SYN Stealth Scan at 12:05
Scanning 192.168.1.8 [65535 ports]
Discovered open port 139/tcp on 192.168.1.8
Discovered open port 135/tcp on 192.168.1.8
Discovered open port 445/tcp on 192.168.1.8
Discovered open port 912/tcp on 192.168.1.8
Discovered open port 49668/tcp on 192.168.1.8
Discovered open port 49672/tcp on 192.168.1.8
Discovered open port 20505/tcp on 192.168.1.8
Discovered open port 49665/tcp on 192.168.1.8
Discovered open port 902/tcp on 192.168.1.8
Discovered open port 50131/tcp on 192.168.1.8
Discovered open port 49664/tcp on 192.168.1.8
Discovered open port 5040/tcp on 192.168.1.8
Discovered open port 49669/tcp on 192.168.1.8
Discovered open port 27080/tcp on 192.168.1.8
Discovered open port 53145/tcp on 192.168.1.8
Discovered open port 8834/tcp on 192.168.1.8
Discovered open port 49703/tcp on 192.168.1.8
Completed SYN Stealth Scan at 12:05, 7.71s elapsed (65535 total ports)
Initiating Service scan at 12:05
Scanning 17 services on 192.168.1.8
WARNING: Service 192.168.1.8:20505 had already soft-matched rtsp, but now soft-matched sip; ignoring second value
Service scan Timing: About 58.82% done; ETC: 12:07 (0:00:38 remaining)
Completed Service scan at 12:08, 137.67s elapsed (17 services on 1 host)
Initiating OS detection (try #1) against 192.168.1.8
Retrying OS detection (try #2) against 192.168.1.8
Retrying OS detection (try #3) against 192.168.1.8
Retrying OS detection (try #4) against 192.168.1.8
Retrying OS detection (try #5) against 192.168.1.8
NSE: Script scanning 192.168.1.8.
Initiating NSE at 12:08
Completed NSE at 12:08, 14.36s elapsed
Initiating NSE at 12:08
NSOCK ERROR [4254.2960s] poll_loop(): nsock_loop error 10022: An invalid argument was supplied. 
NSE: Script Engine Scan Aborted.
An error was thrown by the engine: C:\Program Files (x86)\Nmap/nse_main.lua:1078: a fatal error occurred in nsock_loop
stack traceback:
	[C]: in function 'nmap.socket.loop'
	C:\Program Files (x86)\Nmap/nse_main.lua:1078: in upvalue 'run'
	C:\Program Files (x86)\Nmap/nse_main.lua:1488: in function &lt;C:\Program Files (x86)\Nmap/nse_main.lua:1435&gt;
	[C]: in ?
Nmap scan report for 192.168.1.8
Host is up (0.00073s latency).
Not shown: 65517 closed tcp ports (reset)
PORT      STATE    SERVICE            VERSION
135/tcp   open     msrpc              Microsoft Windows RPC
137/tcp   filtered netbios-ns
139/tcp   open     netbios-ssn        Microsoft Windows netbios-ssn
445/tcp   open     microsoft-ds?
902/tcp   open     ssl/vmware-auth    VMware Authentication Daemon 1.10 (Uses VNC, SOAP)
912/tcp   open     vmware-auth        VMware Authentication Daemon 1.0 (Uses VNC, SOAP)
5040/tcp  open     unknown
8834/tcp  open     ssl/nessus-xmlrpc?
| ssl-cert: Subject: commonName=LAPTOP-T4P8NN90/organizationName=Nessus Users United/stateOrProvinceName=NY/countryName=US
| Issuer: commonName=Nessus Certification Authority/organizationName=Nessus Users United/stateOrProvinceName=NY/countryName=US
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2025-09-09T06:44:08
| Not valid after:  2029-09-08T06:44:08
| MD5:     e861 05ec 1ff6 ddc6 16ac b112 4fab cb25
| SHA-1:   1f46 5f45 faa6 8011 9bb5 d386 af28 7cbd 814b 148b
|_SHA-256: a9bb 1d4c 9b52 cade 599f d758 6f7a 5df1 3c39 8621 0954 8300 c69d 6fc1 9c6c d963
20505/tcp open     rtsp
|_rtsp-methods: ERROR: Script execution failed (use -d to debug)
| fingerprint-strings: 
|   FourOhFourRequest, GetRequest, HTTPOptions: 
|     HTTP/1.0 200 OK
|     Date: Mon, 22 Sep 2025 06:36:00 GMT
|     Connection: Close
|     Content-Type: application/json
|     {"errcode":200,"message":"METHOD_NOT_ALLOWED"}
|   GenericLines: 
|     HTTP/1.1 400 Bad Request
|     Connection: Close
|   RTSPRequest: 
|     RTSP/1.0 200 OK
|     Date: Mon, 22 Sep 2025 06:36:00 GMT
|     Connection: Close
|     Content-Type: application/json
|     {"errcode":200,"message":"METHOD_NOT_ALLOWED"}
|   SIPOptions: 
|     SIP/2.0 200 OK
|     Date: Mon, 22 Sep 2025 06:36:00 GMT
|     Connection: Close
|     Content-Type: application/json
|_    {"errcode":200,"message":"METHOD_NOT_ALLOWED"}
27080/tcp open     flexlm             FlexLM license manager
49664/tcp open     msrpc              Microsoft Windows RPC
49665/tcp open     msrpc              Microsoft Windows RPC
49668/tcp open     msrpc              Microsoft Windows RPC
49669/tcp open     msrpc              Microsoft Windows RPC
49672/tcp open     msrpc              Microsoft Windows RPC
49703/tcp open     msrpc              Microsoft Windows RPC
50131/tcp open     http               Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Bad Request
53145/tcp open     flexlm             FlexLM license manager
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port20505-TCP:V=7.97%I=7%D=9/22%Time=68D0EE50%P=i686-pc-windows-windows
SF:%r(GenericLines,2F,"HTTP/1\.1\x20400\x20Bad\x20Request\r\nConnection:\x
SF:20Close\r\n\r\n")%r(GetRequest,99,"HTTP/1\.0\x20200\x20OK\r\nDate:\x20M
SF:on,\x2022\x20Sep\x202025\x2006:36:00\x20GMT\r\nConnection:\x20Close\r\n
SF:Content-Type:\x20application/json\r\n\r\n{\"errcode\":200,\"message\":\
SF:"METHOD_NOT_ALLOWED\"}")%r(HTTPOptions,99,"HTTP/1\.0\x20200\x20OK\r\nDa
SF:te:\x20Mon,\x2022\x20Sep\x202025\x2006:36:00\x20GMT\r\nConnection:\x20C
SF:lose\r\nContent-Type:\x20application/json\r\n\r\n{\"errcode\":200,\"mes
SF:sage\":\"METHOD_NOT_ALLOWED\"}")%r(RTSPRequest,99,"RTSP/1\.0\x20200\x20
SF:OK\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:36:00\x20GMT\r\nConnecti
SF:on:\x20Close\r\nContent-Type:\x20application/json\r\n\r\n{\"errcode\":2
SF:00,\"message\":\"METHOD_NOT_ALLOWED\"}")%r(FourOhFourRequest,99,"HTTP/1
SF:\.0\x20200\x20OK\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:36:00\x20G
SF:MT\r\nConnection:\x20Close\r\nContent-Type:\x20application/json\r\n\r\n
SF:{\"errcode\":200,\"message\":\"METHOD_NOT_ALLOWED\"}")%r(SIPOptions,98,
SF:"SIP/2\.0\x20200\x20OK\r\nDate:\x20Mon,\x2022\x20Sep\x202025\x2006:36:0
SF:0\x20GMT\r\nConnection:\x20Close\r\nContent-Type:\x20application/json\r
SF:\n\r\n{\"errcode\":200,\"message\":\"METHOD_NOT_ALLOWED\"}");
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.97%E=4%D=9/22%OT=135%CT=1%CU=41036%PV=Y%DS=0%DC=L%G=Y%TM=68D0EE
OS:ED%P=i686-pc-windows-windows)SEQ(SP=105%GCD=1%ISR=109%TI=I%CI=I%II=I%SS=
OS:S%TS=A)SEQ(SP=106%GCD=1%ISR=108%TI=I%CI=I%II=I%SS=S%TS=A)SEQ(SP=107%GCD=
OS:1%ISR=10B%TI=I%CI=I%II=I%SS=S%TS=A)SEQ(SP=107%GCD=1%ISR=10C%TI=I%CI=I%II
OS:=I%SS=S%TS=A)SEQ(SP=F7%GCD=1%ISR=10C%TI=I%CI=I%II=I%SS=S%TS=A)OPS(O1=MFF
OS:D7NW8ST11%O2=MFFD7NW8ST11%O3=MFFD7NW8NNT11%O4=MFFD7NW8ST11%O5=MFFD7NW8ST
OS:11%O6=MFFD7ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=FFFF)ECN(
OS:R=Y%DF=Y%T=80%W=FFFF%O=MFFD7NW8NNS%CC=N%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+%F=A
OS:S%RD=0%Q=)T2(R=Y%DF=Y%T=80%W=0%S=Z%A=S%F=AR%O=%RD=0%Q=)T3(R=Y%DF=Y%T=80%
OS:W=0%S=Z%A=O%F=AR%O=%RD=0%Q=)T4(R=Y%DF=Y%T=80%W=0%S=A%A=O%F=R%O=%RD=0%Q=)
OS:T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=80%W=0%S=A%A
OS:=O%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(R=Y%D
OS:F=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=Z%RUCK=G%RUD=G)IE(R=Y%DFI=N%T=8
OS:0%CD=Z)

Uptime guess: 1.019 days (since Sun Sep 21 11:41:52 2025)
Network Distance: 0 hops
TCP Sequence Prediction: Difficulty=261 (Good luck!)
IP ID Sequence Generation: Incremental
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-security-mode: 
|   3.1.1: 
|_    Message signing enabled but not required
| smb2-time: 
|   date: 2025-09-22T06:38:23
|_  start_date: N/A

NSE: Script Post-scanning.
Initiating NSE at 12:08
NSOCK ERROR [4254.3550s] poll_loop(): nsock_loop error 10022: An invalid argument was supplied. 
NSE: Script Engine Scan Aborted.
An error was thrown by the engine: C:\Program Files (x86)\Nmap/nse_main.lua:1078: a fatal error occurred in nsock_loop
stack traceback:
	[C]: in function 'nmap.socket.loop'
	C:\Program Files (x86)\Nmap/nse_main.lua:1078: in upvalue 'run'
	C:\Program Files (x86)\Nmap/nse_main.lua:1488: in function &lt;C:\Program Files (x86)\Nmap/nse_main.lua:1435&gt;
	[C]: in ?
Read data files from: C:\Program Files (x86)\Nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 254 IP addresses (6 hosts up) scanned in 4254.36 seconds
           Raw packets sent: 625311 (27.519MB) | Rcvd: 712521 (28.890MB)
</output><host comment=""><status state="down"></status><address addr="192.168.1.6" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.7" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.9" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.10" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.11" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.12" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.13" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.14" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.15" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.16" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.17" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.18" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.19" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.20" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.21" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.22" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.23" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.24" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.25" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.26" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.27" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.28" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.29" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.30" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.31" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.32" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.33" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.34" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.35" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.36" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.37" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.38" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.39" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.40" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.41" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.42" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.43" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.44" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.45" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.46" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.47" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.48" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.49" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.50" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.51" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.52" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.53" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.54" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.55" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.56" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.57" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.58" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.59" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.60" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.61" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.62" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.63" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.64" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.65" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.66" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.67" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.68" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.69" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.70" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.71" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.72" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.73" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.74" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.75" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.76" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.77" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.78" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.79" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.80" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.81" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.82" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.83" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.84" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.85" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.86" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.87" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.88" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.89" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.90" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.91" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.92" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.93" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.94" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.95" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.96" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.97" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.98" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.99" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.100" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.101" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.102" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.103" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.104" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.105" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.106" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.107" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.108" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.109" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.110" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.111" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.112" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.113" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.114" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.115" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.116" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.117" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.118" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.119" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.120" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.121" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.122" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.123" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.124" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.125" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.126" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.127" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.128" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.129" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.130" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.131" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.132" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.133" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.134" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.135" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.136" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.137" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.138" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.139" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.140" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.141" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.142" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.143" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.144" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.145" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.146" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.147" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.148" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.149" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.150" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.151" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.152" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.153" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.154" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.155" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.156" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.157" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.158" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.159" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.160" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.161" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.162" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.163" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.164" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.165" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.166" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.167" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.168" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.169" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.170" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.171" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.172" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.173" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.174" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.175" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.176" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.177" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.178" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.179" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.180" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.181" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.182" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.183" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.184" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.185" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.186" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.187" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.188" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.189" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.190" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.191" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.192" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.193" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.194" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.195" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.196" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.197" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.198" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.199" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.200" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.201" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.202" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.203" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.204" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.205" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.206" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.207" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.208" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.209" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.210" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.211" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.212" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.213" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.214" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.215" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.216" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.217" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.218" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.219" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.220" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.221" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.222" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.223" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.224" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.225" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.226" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.227" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.228" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.229" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.230" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.231" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.232" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.233" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.234" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.235" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.236" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.237" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.238" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.239" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.240" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.241" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.242" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.243" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.244" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.245" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.246" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.247" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.248" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.249" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.250" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.251" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.252" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.253" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="down"></status><address addr="192.168.1.254" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports></ports><os></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence></host><host comment=""><status state="up"></status><address addr="192.168.1.1" vendor="" addrtype="ipv4"></address><address addr="60:BD:2C:67:31:C0" vendor="Taicang T&amp;W Electronics" addrtype="mac"></address><hostnames><hostname name="dsldevice.lan" type="PTR"></hostname></hostnames><ports><extraports count="65526" state="filtered"></extraports><port portid="80" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="rtsp"></service></port><port portid="443" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="rtsp"></service></port><port portid="445" protocol="tcp"><state state="closed" reason="reset" reason_ttl="64"></state><service conf="3" method="table" name="microsoft-ds"></service></port><port portid="8008" protocol="tcp"><state state="closed" reason="reset" reason_ttl="64"></state><service conf="3" method="table" name="http"></service></port><port portid="37591" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service></service></port><port portid="49156" protocol="tcp"><state state="closed" reason="reset" reason_ttl="64"></state><service></service></port><port portid="49157" protocol="tcp"><state state="closed" reason="reset" reason_ttl="64"></state><service></service></port><port portid="49160" protocol="tcp"><state state="closed" reason="reset" reason_ttl="64"></state><service></service></port><port portid="49161" protocol="tcp"><state state="closed" reason="reset" reason_ttl="64"></state><service></service></port></ports><os><portused state="open" proto="tcp" portid="80"></portused><portused state="closed" proto="tcp" portid="445"></portused><portused state="closed" proto="udp" portid="39980"></portused><osmatch name="Linux 3.11 - 4.9" accuracy="100" line="66841"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="4.X" accuracy="100"></osclass></osmatch></os><uptime seconds="100257" lastboot="Sun Sep 21 08:14:49 2025"></uptime><tcpsequence index="257" difficulty="Good luck!" values="8FB2E8FD,21C2FB1,DD258830,9B12188F,6BA8151A,BA4B7A02"></tcpsequence><ipidsequence class="All zeros" values="0,0,0,0,0,0"></ipidsequence><tcptssequence class="100HZ" values="98DCD0,98DCDB,98DCE5,98DCF2,98DCFB,98DD05"></tcptssequence><trace proto="" port=""><hop ttl="1" rtt="5.08" ipaddr="192.168.1.1" host="dsldevice.lan"></hop></trace></host><host comment=""><status state="up"></status><address addr="192.168.1.2" vendor="" addrtype="ipv4"></address><address addr="5A:08:F4:EF:5F:2E" vendor="" addrtype="mac"></address><hostnames></hostnames><ports><extraports count="65468" state="closed"></extraports><extraports count="67" state="filtered"></extraports></ports><os><portused state="closed" proto="tcp" portid="1"></portused><portused state="closed" proto="udp" portid="37190"></portused><osmatch name="Microsoft Windows 10 - 11" accuracy="100" line="74431"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="11" accuracy="100"></osclass></osmatch><osmatch name="Microsoft Windows Server 2016" accuracy="100" line="81849"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="2016" accuracy="100"></osclass></osmatch><osmatch name="Microsoft Xbox 360 Dashboard" accuracy="100" line="91139"><osclass vendor="Microsoft" osfamily="Xbox 360" type="media device" osgen="" accuracy="100"></osclass></osmatch><osmatch name="NTI E-MICRO-TRHP temperature sensor" accuracy="100" line="96049"><osclass vendor="NTI" osfamily="embedded" type="specialized" osgen="" accuracy="100"></osclass></osmatch></os><uptime seconds="" lastboot=""></uptime><tcpsequence index="" difficulty="" values=""></tcpsequence><ipidsequence class="" values=""></ipidsequence><tcptssequence class="" values=""></tcptssequence><trace proto="" port=""><hop ttl="1" rtt="226.65" ipaddr="192.168.1.2" host=""></hop></trace></host><host comment=""><status state="up"></status><address addr="192.168.1.3" vendor="" addrtype="ipv4"></address><address addr="68:FC:CA:E6:97:04" vendor="Samsung Electronics" addrtype="mac"></address><hostnames></hostnames><ports><extraports count="65524" state="closed"></extraports><port portid="7000" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="rtsp" product="AirTunes rtspd" version="377.40.00"></service></port><port portid="7678" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="upnp" product="Samsung AllShare upnpd" version="1.0" extrainfo="UPnP 1.1"></service></port><port portid="8001" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="vcom-tunnel"></service></port><port portid="8002" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="teradataordbms"></service></port><port portid="8080" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="http-proxy" product="WebServer"></service></port><port portid="8187" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="upnp" product="Samsung AllShare upnpd" version="1.0" extrainfo="UPnP 1.1"></service></port><port portid="9080" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="glrpc"></service></port><port portid="9197" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="upnp" product="Samsung AllShare upnpd" version="1.0" extrainfo="UPnP 1.1"></service></port><port portid="15500" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service></service></port><port portid="45061" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="unknown"></service></port><port portid="45221" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="8" method="probed" name="tcpwrapped"></service></port></ports><os><portused state="open" proto="tcp" portid="7000"></portused><portused state="closed" proto="tcp" portid="1"></portused><portused state="closed" proto="udp" portid="32062"></portused><osmatch name="Linux 4.15 - 5.19" accuracy="100" line="70534"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="5.X" accuracy="100"></osclass></osmatch></os><uptime seconds="1479073" lastboot="Fri Sep  5 09:14:33 2025"></uptime><tcpsequence index="249" difficulty="Good luck!" values="31BA0117,465642F3,3ACBA049,511F7E34,81A6D5B1,A22AD33D"></tcpsequence><ipidsequence class="All zeros" values="0,0,0,0,0,0"></ipidsequence><tcptssequence class="1000HZ" values="5827B1A0,5827B204,5827B26D,5827B2EB,5827B353,5827B3BF"></tcptssequence><trace proto="" port=""><hop ttl="1" rtt="4.40" ipaddr="192.168.1.3" host=""></hop></trace></host><host comment=""><status state="up"></status><address addr="192.168.1.4" vendor="" addrtype="ipv4"></address><address addr="26:43:1D:FE:39:5C" vendor="" addrtype="mac"></address><hostnames></hostnames><ports><extraports count="65507" state="closed"></extraports><port portid="7" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service conf="3" method="table" name="echo"></service></port><port portid="650" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service conf="3" method="table" name="obex"></service></port><port portid="2101" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service conf="3" method="table" name="rtcm-sc104"></service></port><port portid="3092" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="9894" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="10150" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service></service></port><port portid="10152" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service></service></port><port portid="15075" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="17737" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="19663" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="26127" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="28995" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="31937" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="34409" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="35374" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="39399" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="41413" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="44352" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="44797" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="46627" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="46888" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="unknown"></service></port><port portid="48045" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="48623" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="53236" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="54902" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="58549" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="60827" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port><port portid="65411" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service></service></port></ports><os><portused state="open" proto="tcp" portid="10150"></portused><portused state="closed" proto="tcp" portid="1"></portused><portused state="closed" proto="udp" portid="36984"></portused><osmatch name="Android 10 - 12 (Linux 4.14 - 4.19)" accuracy="100" line="71590"><osclass vendor="Google" osfamily="Android" type="phone" osgen="12.X" accuracy="100"></osclass></osmatch></os><uptime seconds="3699932" lastboot="Sun Aug 10 16:20:14 2025"></uptime><tcpsequence index="259" difficulty="Good luck!" values="9F8A070A,6E4D6D81,52076980,227BE5EF,B02AF3BD,D7C8C004"></tcpsequence><ipidsequence class="All zeros" values="0,0,0,0,0,0"></ipidsequence><tcptssequence class="1000HZ" values="DC874F6B,DC874FCE,DC874FDF,DC8750CB,DC8750CB,DC875131"></tcptssequence><trace proto="" port=""><hop ttl="1" rtt="88.23" ipaddr="192.168.1.4" host=""></hop></trace></host><host comment=""><status state="up"></status><address addr="192.168.1.5" vendor="" addrtype="ipv4"></address><address addr="3A:C0:1F:FA:EE:3A" vendor="" addrtype="mac"></address><hostnames></hostnames><ports><extraports count="65525" state="closed"></extraports><port portid="6091" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="unknown"></service></port><port portid="6466" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="unknown"></service></port><port portid="6467" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="unknown"></service></port><port portid="8008" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="http"></service></port><port portid="8009" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="10" method="probed" name="castv2" product="Ninja Sphere Chromecast driver"></service></port><port portid="8443" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="https-alt"></service></port><port portid="9000" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="3" method="table" name="cslistener"></service></port><port portid="38197" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="8" method="probed" name="tcpwrapped"></service></port><port portid="38231" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="8" method="probed" name="tcpwrapped"></service></port><port portid="40883" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="64"></state><service conf="8" method="probed" name="tcpwrapped"></service></port></ports><os><portused state="open" proto="tcp" portid="6091"></portused><portused state="closed" proto="tcp" portid="1"></portused><portused state="closed" proto="udp" portid="39349"></portused><osmatch name="Android 5.0 - 6.0.1 (Linux 3.4)" accuracy="97" line="33785"><osclass vendor="Linux" osfamily="Linux" type="phone" osgen="3.X" accuracy="97"></osclass></osmatch><osmatch name="Linux 2.6.32" accuracy="96" line="58659"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="2.6.X" accuracy="96"></osclass></osmatch><osmatch name="Linux 4.15" accuracy="96" line="70405"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="4.X" accuracy="96"></osclass></osmatch><osmatch name="OpenWrt 21.02 (Linux 5.4)" accuracy="96" line="72530"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="5.X" accuracy="96"></osclass></osmatch><osmatch name="MikroTik RouterOS 7.2 - 7.5 (Linux 5.6.3)" accuracy="96" line="91792"><osclass vendor="Linux" osfamily="Linux" type="router" osgen="5.X" accuracy="96"></osclass></osmatch><osmatch name="Linux 3.2 - 4.14" accuracy="96" line="68432"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="4.X" accuracy="96"></osclass></osmatch><osmatch name="Linux 4.15 - 5.19" accuracy="96" line="70534"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="5.X" accuracy="96"></osclass></osmatch><osmatch name="Linux 2.6.32 - 3.10" accuracy="96" line="59874"><osclass vendor="Linux" osfamily="Linux" type="general purpose" osgen="3.X" accuracy="96"></osclass></osmatch><osmatch name="Android 9 - 10 (Linux 4.9 - 4.14)" accuracy="96" line="32762"><osclass vendor="Linux" osfamily="Linux" type="phone" osgen="4.X" accuracy="96"></osclass></osmatch><osmatch name="Android 12 (Linux 5.4)" accuracy="96" line="32802"><osclass vendor="Linux" osfamily="Linux" type="phone" osgen="5.X" accuracy="96"></osclass></osmatch></os><uptime seconds="2045761" lastboot="Fri Aug 29 19:49:45 2025"></uptime><tcpsequence index="253" difficulty="Good luck!" values="D25A7BFE,239248E7,96A6F08F,1C95CD6,A31DAF22,DF2EEB0F"></tcpsequence><ipidsequence class="All zeros" values="0,0,0,0,0,0"></ipidsequence><tcptssequence class="1000HZ" values="79EEEAF2,79EEEB4C,79EEEC10,79EEECE6,79EEECE6,79EEECFC"></tcptssequence><trace proto="" port=""><hop ttl="1" rtt="61.36" ipaddr="192.168.1.5" host=""></hop></trace></host><host comment=""><status state="up"></status><address addr="192.168.1.8" vendor="" addrtype="ipv4"></address><hostnames></hostnames><ports><extraports count="65517" state="closed"></extraports><port portid="135" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="msrpc" product="Microsoft Windows RPC"></service></port><port portid="137" protocol="tcp"><state state="filtered" reason="no-response" reason_ttl="0"></state><service conf="3" method="table" name="netbios-ns"></service></port><port portid="139" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="netbios-ssn" product="Microsoft Windows netbios-ssn"></service></port><port portid="445" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="3" method="table" name="microsoft-ds"></service></port><port portid="902" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="vmware-auth" product="VMware Authentication Daemon" version="1.10" extrainfo="Uses VNC, SOAP"></service></port><port portid="912" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="vmware-auth" product="VMware Authentication Daemon" version="1.0" extrainfo="Uses VNC, SOAP"></service></port><port portid="5040" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service></service></port><port portid="8834" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="3" method="table" name="nessus-xmlrpc"></service></port><port portid="20505" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="rtsp"></service></port><port portid="27080" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="flexlm" product="FlexLM license manager"></service></port><port portid="49664" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="msrpc" product="Microsoft Windows RPC"></service></port><port portid="49665" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="msrpc" product="Microsoft Windows RPC"></service></port><port portid="49668" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="msrpc" product="Microsoft Windows RPC"></service></port><port portid="49669" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="msrpc" product="Microsoft Windows RPC"></service></port><port portid="49672" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="msrpc" product="Microsoft Windows RPC"></service></port><port portid="49703" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="msrpc" product="Microsoft Windows RPC"></service></port><port portid="50131" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="http" product="Microsoft HTTPAPI httpd" version="2.0" extrainfo="SSDP/UPnP"></service></port><port portid="53145" protocol="tcp"><state state="open" reason="syn-ack" reason_ttl="128"></state><service conf="10" method="probed" name="flexlm" product="FlexLM license manager"></service></port></ports><os><portused state="open" proto="tcp" portid="135"></portused><portused state="closed" proto="tcp" portid="1"></portused><portused state="closed" proto="udp" portid="41036"></portused><osmatch name="Microsoft Windows 10 1607 - 11 23H2" accuracy="99" line="74791"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="11" accuracy="99"></osclass></osmatch><osmatch name="Microsoft Windows 10 1511" accuracy="97" line="74530"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="10" accuracy="97"></osclass></osmatch><osmatch name="Windows 11 21H2" accuracy="97" line="75587"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="11" accuracy="97"></osclass></osmatch><osmatch name="Microsoft Windows 10 1703" accuracy="96" line="74847"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="10" accuracy="96"></osclass></osmatch><osmatch name="Windows Server 2022" accuracy="96" line="82130"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="2022" accuracy="96"></osclass></osmatch><osmatch name="Microsoft Windows 10 1703 or Windows 11 21H2" accuracy="96" line="74943"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="11" accuracy="96"></osclass></osmatch><osmatch name="Microsoft Windows 10 1703 - 11 21H2" accuracy="95" line="74920"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="11" accuracy="95"></osclass></osmatch><osmatch name="Microsoft Windows 11 21H2" accuracy="95" line="75569"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="11" accuracy="95"></osclass></osmatch><osmatch name="Microsoft Windows 7 or 8.1 R1" accuracy="94" line="82755"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="8.1" accuracy="94"></osclass></osmatch><osmatch name="Microsoft Windows 10 1607" accuracy="94" line="74626"><osclass vendor="Microsoft" osfamily="Windows" type="general purpose" osgen="10" accuracy="94"></osclass></osmatch></os><uptime seconds="88005" lastboot="Sun Sep 21 11:41:52 2025"></uptime><tcpsequence index="261" difficulty="Good luck!" values="A073AA70,F80B787F,59D81979,A9D7925A,B219A5FC,9E31855F"></tcpsequence><ipidsequence class="Incremental" values="1FDC,1FDE,1FE0,1FE2,1FE4,1FE6"></ipidsequence><tcptssequence class="1000HZ" values="53E9D5C,53E9DCB,53E9E35,53E9EA3,53E9F10,53E9F7E"></tcptssequence></host><runstats><finished time="1758523117" timestr="Mon Sep 22 12:08:37 2025"></finished><hosts up="6" down="248" total="254"></hosts></runstats></nmaprun>

Key Takeaways

Full port scans of large networks can take many hours or days.

Adjusting scan scope (fewer hosts, fewer ports) makes results more practical.

Documenting the process is as important as the scan itself.
