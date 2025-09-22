Network Scan Project

This project demonstrates the use of Nmap/Zenmap for network scanning.

Tools Used

Nmap (command-line)

Zenmap (GUI for Nmap)


Methodology

1. Attempted a full TCP scan on all 65,535 ports across the subnet 192.168.1.1-254 using:

nmap -p 1-65535 -T4 -A -v 192.168.1.1-254

This scan was very large and took a long time to complete.
2. Saved partial results from Zenmap after several hours of scanning.

Example: some hosts (e.g., 192.168.1.5, 192.168.1.14) showed open ports such as 80, 443, 8009, 8080, 3306.



3. Learned that in real environments, it is better to:

Limit scans to top 1000 ports (default Nmap behavior), or

Scan specific ports (e.g., 22, 80, 443, 3306) for faster results.




Results

The raw scan output is saved in "C:\Users\Udaykiran\Starting Nmap 7.97 ( httpsnmap.org.txt"

Key Takeaways

Full port scans of large networks can take many hours or days.

Adjusting scan scope (fewer hosts, fewer ports) makes results more practical.

Documenting the process is as important as the scan itself.
