Welcome back, ready to dive right in? So unlike protocols like DNS and
DHCP, network address translation or NAT, is a technique instead
of a defined standard. This means that some of what we'll
discuss in this lesson might be more high level than some of our other topics. Different operating systems and
different network hardware vendors have implemented the details
of NAT in different ways, but the concepts of what it
accomplishes are pretty constant. Network address translation does
pretty much what it sounds like, it takes one IP address and
translates it into another. There are lots of reasons why
you would want to do this. They range from security safeguards
to preserving the limited amounts of available IPv4 space. We'll discuss the implications of NAT and the IPv4 address space
later in this lesson. But for now, let's just focus
on how NAT itself works and how it can provide additional
security measures to a network. At its most basic level,
NAT is a technology that allows a gateway, usually a router or firewall, to rewrite
the source IP of an outgoing IP datagram while retaining the original IP in
order to rewrite it into the response. To explain this better,
let's look at a simple NAT example. Let's say we have two networks. Network A consists of
the 10.1.1.0/24 address space and network B consists of
the 192.168.1.0/24 address space. Sitting between these
networks is a router that has an interface on network
A with an IP of 10.1.1.1 and an interface on network B of 192.168.1.1. Now, let's put two computers
on these networks. Computer 1 is on network A and
has an IP of 10.1.1.100. And computer 2 is on network B and has an IP of 192.168.1.100. Computer 1 wants to communicate
with a web server on computer 2. So it crafts the appropriate
packet at all layers and sends this to its primary gateway, the
router sitting between the two networks. So far, this is a lot like many of our
earlier examples, but in this instance, the router is configured to perform
NAT for any outbound packets. Normally, a router will inspect
the contents of an IP datagram, decrement the TTL by 1,
re-calculate the checksum, and forward the rest of the data at
the network layer without touching it. But with NAT, the router will also
rewrite the source IP address, which in this instance, becomes the
router's IP on network B or 192.168.1.1. When the datagram gets to computer 2, it'll look like it originated from
the router, not from computer 1. Now, computer 2 crafts its response and
sends it back to the router. The router, knowing that this
traffic is actually intended for computer 1, rewrites the destination
IP field before forwarding it along. What NAT is doing in this example, is hiding the IP of
computer 1 from computer 2. This is known as IP masquerading. IP masquerading is
an important security concept. The most basic concept at play
here is that no one can establish a connection to your computer if they
don't know what IP address it has. By using NAT in the way
we've just described, we could actually have hundreds
of computers on network A, all of their IPs being translated
by the router to its own. To the outside world, the entire address
space of network A is protected and invisible. This is known as one-to-many NAT, and you'll see it in use
on lots of LANs today.
