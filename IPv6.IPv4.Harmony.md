It's just not possible for
the entire Internet and all connected networks to
switch to IPv6 all at once. There would be way too
much coordination at play. Too many old devices that might not
even know how to speak IPv6 at all, still requiring connections. So the only way IPv6 will ever
take hold is to develop a way for IPv6 and
IPv4 traffic to coexist at the same time. This would let individual organizations
make the transition when they can. One example of how this can work is with
what's known as IPv4 mapped address space. The IPv6 specifications have
set aside a number of addresses that can be directly
correlated to an IPv4 address. Any IPv6 address that begins with
80 zeros, and is then followed by 16 ones is understood to be part
of the IPv4 mapped address space. The remaining 32 bits
of the IPv6 address is just the same 32 bits of the IPv4
address it's meant to represent. This gives us a way for IPv4 traffic
to travel over an IPv6 network. But probably more important is for IPv6 traffic to have a way to
travel over IPv4 networks. It's easier for an individual organization
to make the move to IPv6 than it is for the networks at the core
of the Internet to. So while IPv6 adoption
becomes more widespread, it'll need a way to travel over the old
IPv4 remnants of the Internet backbone. The primary way this is achieve
today is through IPv6 tunnels. IPv6 tunnels are conceptually
pretty simple. They consist of IPv6 tunnels servers
on either end of a connection. These IPv6 tunnel servers take
incoming IPv6 traffic and encapsulate it within
traditional IPv4 datagrams. This is then delivered across
the IPv4 Internet space where it's received by another IPv6 tunnel server. That server performs
the de-encapsulation and passes the IPv6 traffic
further along in the network. Along with IPv6 tunnel technologies, the concept of an IPv6 tunnel
broker has also emerged. These are companies that provide
IPv6 tunneling endpoints for you, so you don't have to introduce
additional equipment to your network. There are a lot of competing protocols to
be used for these kinds of IPv6 tunnels. Since this is still a new and
evolving space, it's not clear who the winner will be. I've left you with some links to
read about the main competitors right after this video. It doesn't really matter
which tunneling technology ends up becoming the most common solution. It'll probably fade away in time itself. The future of networking is the adoption
of IPv6 as the main protocol at the network layer, and
one day we won't need any tunnels at all. The future is limitless, and
tunnelless, or something like that. You've done an amazing job at getting
through all this information. So take some time to pat
yourself on the back. You've got one final quiz and
a final project to get through. And then you can check this
course off your to do list. Are you starting to see the light
at the end of the tunnel?
