IP addresses can be split into two
sections, the network ID and the host ID. Earlier we mentioned that IBM owns
all IP addresses that have a nine as the value of the first
octet in an IP address. If we take an example IP address of
9.100.100.100, the network ID would be the first octet, and the host ID would
be the second, third and fourth octets. The address class system is a way
of defining how the global IP address space is split up. There are three primary
types of address classes. Class A, Class B and Class C. Class A addresses are those where
the first octet is used for the network ID and
the last three are used for the host ID. Class B addresses are where the first
two octets are used for the network ID, and the second two are used for
the host ID. Class C addresses,
as you might have guessed, are those where the first three octets
are used for the network ID, and only the final octet is used for
the host ID. Each address class represents
a network of vastly different size. For example, since a Class A network has
a total of 24 bits of host ID space, this comes out to 2 to the 24th or
16,777,216 individual addresses. Compare this with a Class C network which
only has eight bits of host ID space. For a Class C network, this comes out
to 2 to the 8th or 256 addresses. You can also tell exactly what
address class in IP address belongs to just by looking at it. If the very first bit of an IP address
is 0, it belongs to a Class A network. If the first bits are 10,
it belongs to a Class B network. Finally, if the first bits are 110,
it belongs to a Class C network. Since humans aren't great
at thinking in binary, it's good to know that this also
translates nicely to how these addresses are represented in
dotted decimal notation. You might remember that each octet
in an IP address is eight bits, which means each octet can take
a value between 0 and 255. If the first bit has to be a 0,
as it is with the Class A address, the possible values for
the first octet are 0 through 127. This means that any IP address with
a first octet with one of those values is a Class A address. Similarly, Class B addresses
are restricted to those that begin with the first octet value of 128 through 191. And Class C addresses begin with
the first octet value of 192 through 223. You might notice that this doesn't
cover every possible IP address. That's because there are two
other IP address classes, but they're not quite as
important to understand. Class D addresses always begin with the
bits 1110, and are used for multicasting, which is how a single IP datagram can
be sent to an entire network at once. These addresses begin with decimal
values between 224 and 239. Lastly, Class E addresses make up
all of the remaining IP addresses. But they are unassigned and
only used for testing purposes. In practical terms, this class system has
mostly been replaced by a system known as CIDR or classless inter-domain routing. But the address class system is still in
place in many ways and is important to understand for anyone looking for
a well routed networking education. And you know we're all about that. So, don't worry,
we'll be covering CIDR in a future lesson.
