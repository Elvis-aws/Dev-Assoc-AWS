
# CNAME
- A CNAME (Canonical Name) record is a type of DNS (Domain Name System) record that maps an alias hostname to the real 
  or canonical hostname. This allows a subdomain to be pointed to another domain or subdomain, effectively redirecting 
  all requests to the canonical hostname
- It's important to note that a CNAME record can't be used to point to an IP address, only a domain or subdomain. Also, 
  the domain or subdomain specified in the CNAME record must have its DNS record, typically an A or AAAA record, that 
  contains the IP address that the domain or subdomain resolves to
1. CNAME records can't point to an IP address, only a domain or subdomain
2. CNAME records can't be used in the root domain
3. CNAME records can cause a delay in DNS resolution
4. CNAME records can't coexist with other types of records, such as MX, NS or SOA.