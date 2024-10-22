<h1>Network Analysis with tcpdump</h1>

<h2>Scenario</h2>

<i>This scenario is based on a fictional event.</i>

I'm a cybersecurity analyst working at a company that specializes in providing IT services for clients. Several customers of clients reported that they were not able to access the client company website www.yummyrecipesforme.com, and saw the error “destination port unreachable” after waiting for the page to load. 

I am tasked with analyzing the situation and determining which network protocol was affected during this incident. To start, I attempted to visit the website and I also receive the error “destination port unreachable.” To troubleshoot the issue, I loaded my network analyzer tool, tcpdump, and attempt to load the webpage again. To load the webpage, my browser sends a query to a DNS server via the UDP protocol to retrieve the IP address for the website's domain name; this is part of the DNS protocol. My browser then uses this IP address as the destination IP for sending an HTTPS request to the web server to display the webpage. The analyzer shows that when I send UDP packets to the DNS server, I receive ICMP packets containing the error message: “udp port 53 unreachable.” log from tcpdump packet data. Here's my [network traffic analysis](https://github.com/dainecryption/NetworkAnalysiswithtcpdump/blob/main/Network%20Analysis%20with%20tcpdump.pdf)

![LKXsnNIhT0e1mAz5AEvxog_d363c94e0a4f4a8b90b0be403f6ee1f1_mMBaLWLyXG2omYBcSdjuR8y5_S59zow1ZEPYdjNyJzA1B0r55nI9KmDosI8QHXcEwE51NxM3N5gNtMgSOyVDHyJVLZvZA7_jJtkzUKfxuqFUJPHs57vVVES-LbG5teR8eir4idaqsxFaYJhhVJZn-a_S-txb](https://github.com/user-attachments/assets/6973e1d3-6598-4c8d-94e0-c83d24af373c)

<br />
