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

# DNS Views
DNS views are a feature of some DNS server software that allow different responses to be provided for the same query based on predefined criteria. This feature is particularly useful in scenarios where the DNS server needs to serve different sets of clients or provide different responses based on the source of the DNS query.

Here's how DNS views work:

1. **Client-Specific Responses**: DNS views enable the server to provide different responses to DNS queries from different clients or networks. For example, a DNS server could be configured to provide different IP addresses for the same domain name depending on whether the query comes from an internal network or the public internet.

2. **Geographical Responses**: DNS views can also be used to provide different responses based on the geographical location of the client making the DNS query. This is often used to direct users to the closest or most appropriate server based on their location, improving performance and user experience.

3. **Split DNS**: Another common use case for DNS views is split DNS, where different sets of DNS records are served to internal and external clients. This allows organizations to provide different access policies or resources to internal users compared to external users.

4. **Conditional Responses**: DNS views can be configured to provide conditional responses based on various criteria such as time of day, network conditions, or specific attributes of the DNS query.

DNS views are typically implemented in DNS server software such as BIND (Berkeley Internet Name Domain) and can be configured using specific syntax or configuration options provided by the DNS server software. Properly configuring DNS views can help organizations optimize their DNS infrastructure for performance, security, and compliance with specific requirements.
