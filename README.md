# Circumnavigate Geo-blocking without VPN faff.

Having moved outside of the UK I wanted to be able to access UK services without the faff of VPNs.

SmartDNS is a service that provides a geo based DNS. Create an account at [SmartDNS](https://www.smartdnsproxy.com/), and follow their setup instructions.

You can use the DNS nameservers provided for system wide settings or use a more granular approach using ```resolver```.

## Granular control for MacOS

Create a file for each domain that you want to resolve through the SmartDNS nameserver and place in ```/etc/resolver/```.

Add new domains by naming file according to domain, ie ```co.uk```.

```bash
domain co.uk
search co.uk
nameserver 35.178.60.174
nameserver 46.166.189.68
```