Supplemental Reading for Testing Port Connectivity
Sometimes, you need to know if network connectivity is working at the transport layer. For this, there are two super powerful tools at your disposal: Netcat (nc) on Linux and macOS, and Test-NetConnection on Windows. 

The Netcat tool can be run through the command nc, and has two mandatory arguments, a host and a port. Running this command would try to establish a connection on port 80 to google.com:


If the connection fails, the command will exit. If it succeeds, you'll see a blinking cursor, waiting for more input. This is a way for you to actually send application layer data to the listening service from your own keyboard. If you're really only curious about the status of a report, you can issue the command, with a -z flag, which stands for zero input/output mode. A -v flag, which stands for verbose, is also useful in this scenario. So now, the command looks like this:


By issuing the netcat command with the -Z and -V flags, the command's output will simply tell you if a connection to the port in question is possible or not, like this:


On Windows, Test-NetConnection is a command with some similar functionality. If you run Test-NetConnection with only a host specified, it will default to using an ICMP echo request, much like the program ping. But, it will display way more data, including the data link layer protocol being used. When you issue Test-NetConnection with the -Port flag, you can ask it to test connectivity to a specific port. For example, this command tests a TCP connection to google.com:


Test-NetConnection will return output that looks something like this: 


It's important to call out that both netcat and Test-NetConnection are way more powerful than the brief port connectivity examples we've covered here. In fact, they're such complex tools that covering all of their functionality would be too much for one video. You should read up about all of the other things these super powerful tools can do in the Wikipedia article for Netcat (nc), and in the documentation for Test-NetConnection.