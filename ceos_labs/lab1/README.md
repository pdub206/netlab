## cEOS Lab v1

The lab will be built with five Arista cEOS devices.  They are in a hub and spoke topology with ceos1 being the hub.

Login credentials are admin/admin.

Lab objectives:

1. Configure IPv4 addresses on each interface.  Device ceos1 should always have .1 and the other device should use their device number.
2. Create a loopback on each device using the IP's shown in the topology image.
3. Verify reachability by pinging across each link.
4. Configure BGP on each device using ASN's 100-500.
5. Verify BGP neighbors are in an established state.
6. Advertise loopback IP's to neighbors.
7. Create a route map on ceos1 that denies sending the loopback IP of ceos4 to ceos5.
8. Create a route map on ceos2 that only imports the loopback IP of ceos3.
9. Create a link between ceos2 and ceos3, then form BGP neighbors across this link.
10. Only advertise the ceos2 loopback IP to ceos3.
11. Verify reachability of loopback IP's from all devices.

Bonus points:

1. Use Ansible collection arista.eos to automate the lab objectives above.