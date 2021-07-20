So far, we've discussed ways for one device to transmit
data to one other device. This is what's known as unicast. A unicast transmission is always meant for
just one receiving address. At the Ethernet level, this is done by looking at a special
bit in the destination MAC address. If the least significant bit in the first
octet of a destination address is set to zero, it means that Ethernet frame is
intended for only the destination address. This means it would be sent to all
devices on the collision domain, but only actually received and
processed by the intended destination. If the least significant bit in
the first octet of a destination address is set to one, it means you're
dealing with a multicast frame. A multicast frame is similarly set to
all devices on the local network signal. What's different is that it will be
accepted or discarded by each device depending on criteria aside from
their own hardware MAC address. Network interfaces can be configured
to accept lists of configured multicast addresses for these sort of communication. The third type of Ethernet
transmission is known as broadcast. An Ethernet broadcast is sent
to every single device on a LAN. This is accomplished by using a special
destination known as a broadcast address. The Ethernet broadcast address is all Fs. Ethernet broadcasts are used so that
devices can learn more about each other. Don't worry, you'll be learning
more about broadcast and a technology known as address resolution
protocol later in this course. But for now, let's move on to
dissecting the Ethernet frame.
