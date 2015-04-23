# grepip
[CLI] a simple bash script to filter in IPv4 addresses using GNU grep, one per line

## Examples

$ nslookup rackspace.com
Server:		10.0.1.1
Address:	10.0.1.1#53

Non-authoritative answer:
Name:	rackspace.com
Address: 173.203.44.122


$ nslookup rackspace.com | grepip
10.0.1.1
10.0.1.1
173.203.44.122


$ nslookup rackspace.com | grepip -x
173.203.44.122
