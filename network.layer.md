On a local area network or LAN, nodes can communicate with each other
through their physical MAC addresses. This works well on small scale because
switches can quickly learn the MAC addresses connected to each other ports
to forward transmissions appropriately. But MAC addressing isn't
a scheme that scales well, every single network interface on
the planet has a unique MAC address and they aren't ordered in any systematic way. There is no way of knowing where on
the planet a certain MAC address might be at any one point in time, so it's not
ideal for communicating across distances. Later on in this lesson, when we introduce
ARP or Address Resolution Protocol, you'll see that the way that nodes learn
about each other's physical addressing isn't translatable to anything besides
a single network signet anyway. Clearly we need another solution,
and that is the network layer, and the internet protocol or IP in the IP
addresses that come along with it. By the end of this lesson you'll be
able to take identify an IP address, describe how IP datagrams are encapsulated
inside the payload of an ethernet frame and correctly identify and describe
the many fields of an IP datagram header.
