---
layout: default
---

# Domain Name System (DNS)

***

The Domain Name System (DNS) is a hierarchical and distributed naming system that translates human-readable domain names into IP addresses, enabling users to access websites easily.

- [How Does DNS Work](#how-does-dns-work)

## How Does DNS Work

The DNS process can be broken down into several steps, ensuring that users can access websites by simply typing a domain name into their browser.

1. User Input: You enter a website address (for example, www.geeksforgeeks.org) into your web browser.

2. Local Cache Check: Your browser first checks its local cache to see if it has recently looked up the domain. If it finds the corresponding IP address, it uses that directly without querying external servers.

3. DNS Resolver Query: If the IP address isn’t in the local cache, your computer sends a request to a DNS resolver. The resolver is typically provided by your Internet Service Provider (ISP) or your network settings.

4. Root DNS Server: The resolver sends the request to a root DNS server. The root server doesn’t know the exact IP address for tyler-nse.github.io but knows which Top-Level Domain (TLD) server to query based on the domain’s extension (e.g., .io).

5. TLD Server: The TLD server for .io directs the resolver to the authoritative DNS server for github.io.

6. Authoritative DNS Server: This server holds the actual DNS records for github.io, including the IP address of the website’s server. It sends this IP address back to the resolver.

7. Final Response: The DNS resolver sends the IP address to your computer, allowing it to connect to the website’s server and load the page.

[back](/fundamentals/networks_and_security.html)