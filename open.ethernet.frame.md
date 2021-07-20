To wrap up, we'll round out your
understanding of the basics of networking, by dissecting and Ethernet frame. Understanding the networking basics is
the first step in building a really strong foundation of networking knowledge
that you'll need in IT support. A data packet is an all-encompassing term that represents any single set of binary
data being sent across a network link. The term data packet isn't tied to
any specific layer or technology. It just represents a concept. One set of data being sent
from point A to Point B. Data packets at the Ethernet level
are known as Ethernet frames. An Ethernet frame is a highly
structured collection of information presented in a specific order. This way network interfaces at
the physical layer can convert a string of bits, travelling across a link into
meaningful data or vice versa. Almost all sections of an Ethernet
frame are mandatory and most of them have a fixed size. The first part of an Ethernet
frame is known as the preamble. A preamble is 8 bytes or 64 bits long and
can itself be split into two sections. The first seven bytes are a series
of alternating ones and zeros. These act partially as
a buffer between frames and can also be used by the network interfaces
to synchronize internal clocks they use, to regulate the speed at
which they send data. This last byte in the preamble is known
as the SFD or start frame delimiter. This signals to a receiving device
that the preamble is over and that the actual frame
contents will now follow. Immediately following
the start frame delimiter, comes the destination MAC address. This is the hardware address
of the intended recipient. Which is then followed by
the source MAC address, or where the frame originated from. Don't forget that each MAC address
is 48 bits or 6 bytes long. The next part of an Ethernet frame
is called the EtherType field. It's 16 bits long and used to describe
the protocol of the contents of the frame. We'll be doing a deep dive on what
these protocols are a little later. It's worth calling out that
instead of the EtherType field, you could also find what's
known as a VLAN header. It indicates that the frame itself
is what's called a VLAN frame. If a VLAN header is present,
the EtherType field follows it. VLAN stands for virtual LAN. It's a technique that lets you
have multiple logical LANs operating on the same physical equipment. Any frame with a VLAN tag
will only be delivered out of a switch interface configured
to relay that specific tag. This way you can have a single
physical network that operates like it's multiple LANs. VLANs are usually used to segregate
different forms of traffic. So you might see a company's IP
phones operating on one VLAN, while all desktops operate on another. After this, you'll find a data
payload of an Ethernet frame. A payload in networking terms is
the actual data being transported, which is everything that isn't a header. The data payload of
a traditional Ethernet frame can be anywhere from
46 to 1500 bytes long. This contains all of the data from higher
layers such as the IP, transport and application layers that's
actually being transmitted. Following that data we have what's
known as a frame check sequence. This is a 4-byte or 32-bit number
that represents a checksum value for the entire frame. This checksum value is
calculated by performing what's known as a cyclical
redundancy check against the frame. A cyclical redundancy check or
CRC, is an important concept for data integrity and is used all over
computing, not just network transmissions. A CRC is basically a mathematical
transformation that uses polynomial division to create a number that
represents a larger set of data. Anytime you perform a CRC
against a set of data, you should end up with
the same checksum number. The reason it's included
in the Ethernet frame is so that the receiving network interface can
infer if it received uncorrupted data. When a device gets ready
to send an Internet frame, it collects all the information we
just covered, like the destination and originating MAC addresses,
the data payload and so on. Then it performs a CRC against that data
and attaches the resulting checksum number as the frame check sequence
at the end of the frame. This data is then sent across a link and
received at the other end. Here, all the various fields of
the Ethernet frame are collected and now the receiving side performs
a CRC against that data. If the checksum computed by the receiving
end doesn't match the checksum in the frame check sequence field,
the data is thrown out. This is because some amount of
data must have been lost or corrupted during transmission. It's then up to a protocol at
a higher layer to decide if that data should be retransmitted. Ethernet itself only
reports on data integrity. It doesn't perform data recovery. You've gotten the basics of
networking now, nice work. Next up is a quiz. You got this, but even if you don't, just review the material until you
get more comfortable with this stuff.
