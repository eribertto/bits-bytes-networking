Long before DNS was an established and
globally available technology, it was clear to computer operators that
they needed a language based system to refer to network devices. We've talked about how humans are way
better at remembering descriptive words than numbers, but numbers represent the natural way
that computers think and communicate. The original way that numbered network
addresses were correlated with words was through hosts files. A host file is a flat file that contains,
on each line, a network address followed
by the host name. It can be referred to as. For example, a line in a host file
might read 1.2.3.4 webserver. This means that on the computer where
this host file resides, a user could just refer to webserver instead of
the IP one dot two dot three dot four. Hosts files are evaluated by the
networking stack of the operating system itself. That means the presence of an entry
there would translate to anywhere you might refer to a networking address. Sticking with our earlier example,
a user could type web server into a web browser URL bar, or could issue
a Ping web webserver command and it would get translated to one dot two
dot three dot four in either case. Hosts files might be ancient technology,
but they've stuck around all this time. All modern operating systems,
including those that power our phone and tablets, still have hosts files. One reason is because of a special
IP address we haven't covered yet. The loopback address. A loopback address always
points to itself, so a loopback address is a way of
sending network traffic to yourself. Sending traffic to a loop back
address bypasses all network infrastructure itself and
traffic like that never leaves the node. The loop back IP for
IPV 4 is 127.0.0.1 and it's still to this day
configured on every modern operating system through
an entry in a hosts file. Almost every hosts file in
existence will in the very least, contain a line that reads
127.0.0.1 localhost. Most likely followed
by ::1 localhost where ::1 is the loop back address for IPv 6. Since DNS is everywhere,
hosts files aren't used much anymore, but they still exist and
they're still important to know about. Some software even requires specific
entries in the hosts file to operate properly as antiquated as
this practice may seem. Finally, host files are a popular way for
computer viruses to disrupt and redirect users' traffic. It's not a great idea to use
host files today, but they do have some useful troubleshooting purposes
that can be helpful in IT support. Host files are examined before
a DNS resolution attempt occurs on just about every
major operating system. This let's you force an individual
computer to think a certain domain name always points at a specific IP, got it? We've covered a lot, so
take time to go back if you need to. And make sure you understand
the concepts we're discussing. Next up a short quiz.
