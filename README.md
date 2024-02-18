# Using SmartDNS with MacOS to Circumnavigate Geo-blocking

Having moved outside of the UK I wanted to be able to access UK services without the faff of VPNs.

SmartDNS is a service that provides a geo based DNS. You can use the DNS server provided for system wide settings or use a more granular approach using '''resolver'''.

## Create resolver for each domain

Place these files in '''/etc/resolver/'''.

Add new domains by naming file according to domain, ie '''co.uk'''.

Place following inside the file and save;

domain '''TLD'''
search '''TLD'''
nameserver 35.178.60.174
nameserver 46.166.189.68
