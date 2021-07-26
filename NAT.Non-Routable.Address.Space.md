The IANA has been in charge of
distributing IP addresses since 1988. Since that time, the internet has
expanded at an incredible rate. The 4.2 billion possible IPv4 addresses
have been predicted to run out for a long time and they almost have. For some time now, the IANA has primarily
been responsible with assigning address blocks to the five regional
internet registries or RIRs. The five RIRs are AFRINIC,
which serves the continent of Africa, ARIN which serves the United States,
Canada and parts of the Caribbean. APNIC, which is responsible for most of Asia, Australia and
New Zealand and Pacific Island nations. LACNIC which covers Central and
South America and any parts of the Caribbean
not covered by ARIN. And finally RIPE,
which serves Europe, Russia and the Middle East and
portions of Central Asia. These five RIRs have been responsible for
assigning IP address blocks to organizations within their geographic
areas and most have already run out. The IANA assigned the last unallocated
slash eight network blocks to various RIRs on February 3rd, 2011. Then in April 2011,
APNIC ran out of addresses. RIPE was next, in September of 2012. LACNIC ran out of addresses
to assign in June 2014. And ARIN did the same in September 2015. Only AFNIC has some IPs left, but those
are predicted to be depleted by 2018. Wikipedia has a great article
all about IPv4 exhaustion and the timelines involved. I've added a link to it in
the reading just after this video. This is of course,
a major crisis for the internet. IPv6 will eventually
resolve these problems and we'll covered in more detail
later in this course. But implementing IPv6 worldwide
is going to take some time. For now, we wanted to continue to grow and
we want more people and devices to connect to it but without IP addresses
to assign, a workaround is needed. Spoiler alert, you already know about
the major components of this workaround. NAT and non-routable address space. Remember that non-routable address
space was defined in RFC1918 and consists of several different
IP ranges that anyone can use. And unlimited number of networks can use
non-routable address space internally because internet routers
won't forward traffic to it. This means there's never any
global collision of IP addresses when people use those address spaces. Non-routable address space
is largely usable today because of technologies like NAT. With NAT, you can have hundreds even thousands of
machines using non-routable address space. Yet, with just a single public IP, all those computers can still send traffic
to and receive traffic from the internet. All you need is one single
IPv4 address and via NAT, a router with that IP can represent
lots and lots of computers behind it. It's not a perfect solution, but until
IPv6 becomes more globally available, non-routable address space and
NAT will have to do
