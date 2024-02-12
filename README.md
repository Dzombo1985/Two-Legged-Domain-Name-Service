# Two-Legged-Domain-Name-Service
DNS Configuration for internal (private) &amp; external (public) resolution using views

What is DNS?
DNS stands for Domain Name System. It is a hierarchical decentralized naming system for computers, services, or any resource connected to the Internet or a private network. DNS translates domain names, which are easy-to-remember labels for websites, into the numerical IP addresses needed for locating and identifying computer services and devices with the underlying network protocols.

DNS operates as a distributed database system. When you type a domain name (e.g., www.dzitu.com) into your web browser, your device sends a request to a DNS server to resolve that domain name into the corresponding IP address. DNS servers then work to find the correct IP address associated with the domain name and return it to your device, allowing it to connect to the desired website or service.

DNS plays a crucial role in the functionality of the internet and is essential for navigating the web and accessing various online resources.

DNS resolution can be classified into two main categories: internal (or private) resolution and external (or public) resolution.

1. **Internal (Private) Resolution:**
   - Internal DNS resolution occurs within a private network, such as a corporate intranet or a home network.
   - In this scenario, DNS servers are typically configured to resolve domain names for resources within the network, such as internal websites, servers, and services.
   - The DNS server responsible for internal resolution may be hosted within the organization's network infrastructure, providing fast and efficient name resolution for local resources.
   - Internal DNS servers can be configured to store records for internal resources and may also forward requests for external domain names to external DNS servers if necessary.
   - Security and access control measures can be applied to internal DNS servers to restrict access to sensitive resources within the network.

2. **External (Public) Resolution:**
   - External DNS resolution involves resolving domain names that are accessible from the public internet.
   - When a user or device on a network requests the IP address for an external domain name, the DNS server responsible for external resolution queries authoritative DNS servers on the internet to obtain the corresponding IP address.
   - Authoritative DNS servers are responsible for storing and providing authoritative information about domain names and their associated IP addresses.
   - External DNS resolution is critical for accessing websites, services, and resources hosted outside of the local network, such as popular websites, online services, and cloud-based applications.
   - External DNS servers, often provided by internet service providers (ISPs) or public DNS providers like Google DNS or Cloudflare DNS, handle requests for domain names outside of the local network.

In summary, internal DNS resolution handles domain names within a private network, while external DNS resolution deals with domain names accessible from the public internet. Both types of resolution are essential for efficient and secure communication within and outside of an organization's network infrastructure.
