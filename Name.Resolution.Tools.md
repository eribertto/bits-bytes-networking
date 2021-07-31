Name resolution is an important
part of how the Internet works. Most of the time, your operating
system handles all look ups for you. But as an IT support specialist,
sometimes it can be useful to run these queries yourself, so you can see exactly
what's happening behind the scenes. Luckily, there are lots of different
command line tools out there to help you with this. The most common tool is known as nslookup. And it's available on all three of the
operating systems we've been discussing, Linux, Mac, and Windows. A basic use of nslookup is pretty simple. You execute the nslookup command
with the host name following it. And the output displays what server
was used to perform the request and the resolution result. Let's say you needed to know
the IP address for a twitter.com. You would just enter nslookup twitter.com
and the A record would be returned. Nslookup is way more
powerful than just that. It includes an interactive mode that
lets you set additional options and run lots of queries in a row. To start an interactive nslookup session, you just enter nslookup,
without any hostname following it. You should see an angle
bracket acting as your prompt. From interactive mode,
you can make lots of requests in a row. You can also perform some extra
configuration to help with more in-depth trouble shooting. While in interactive mode,
if you type server, then an address, all the following name
resolution queries will be attempted to be made using that server
instead of the default name server. You can also enter set type=
followed by a resource record type. By default,
nslookup will return A records. But this lets you explicitly ask for
AAAA or MX or even text records
associated with the host. If you really want to see exactly what's
going on, you can enter set debug. This will allow the tool to
display the full response packets, including any intermediary requests and
all of their contents. Warning, this is a lot of data and can contain details like the TTL left,
if it's a cached response, all the way to the serial number of the
zone file the request was made against.
