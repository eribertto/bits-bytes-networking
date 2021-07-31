Supplemental Reading for IPv6 and IPv4 Harmony
While IPv6 adoption becomes more widespread, it'll need a way to travel over the old IPv4 remnants of the Internet backbone. The primary way this is achieved today is through IPv6 tunnels. IPv6 tunnels are conceptually pretty simple. They consist of IPv6 tunnel servers on either end of a connection. These IPv6 tunnel servers take incoming IPv6 traffic and encapsulate it within traditional IPv4 datagrams. This is then delivered across the IPv4 Internet space where it's received by another IPv6 tunnel server. That server performs the de-encapsulation and passes the IPv6 traffic further along in the network.

There are a lot of competing protocols to be used for these kinds of IPv6 tunnels. Since this is still a new and evolving space, it's not clear who the winner will be. Some of the main competitors are 6in4, Tunnel Setup Protocol, and Anything in Anything (AYIYA).

