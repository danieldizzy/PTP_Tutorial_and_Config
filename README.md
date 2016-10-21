# Linux PTP Config
General documentation and source about PTP

## Ubuntu PTP Config
### IEEE1588 Linux PTP
![Penguin Time](/Tux.png?raw=true "Tux")

#### What is PTP
Linux PTP is a software implementation of PrecisionTime Protocol (PTP) that is in accordance with the IEEE 1588standard.  Linux PTP makes use of the Linux kernel, this allowed usto take advantage of the flexibility that is inherent to LinuxApplication Programming Interfaces (API).  Another very practicalreason for our choice was cost.  Linux PTP is free and readilyavailable for download. Some useful features of Linux PTP are as follows.

* Supports hardware and software time stamping via the Linux SO_TIMESTAMPING socket option.    
* Supports the Linux PTP Hardware Clock (PHC) subsystem by using the clock_gettime family of calls, including the new clock_adjtimex    system call.    
* Implements Boundary Clock (BC) and Ordinary Clock (OC).    
* Transport over UDP/IPv4, UDP/IPv6, and raw Ethernet (Layer 2).    
* Supports IEEE 802.1AS-2011 in the role of end station.    
* Modular design allowing painless addition of new transports and clock servos.

Generally, it is best to avoid building software from source to be installed. For the sake of understanding building from source is not a bad choice. That is the reason i decided to follow these steps. I found some useful sources which will be added to this tutorial.



##[Introduction to PTP from redhat](https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/6/html/Deployment_Guide/ch-Configuring_PTP_Using_ptp4l.html)

The machine requirements for Linux PTP implementation     
* Linux kernel version 3.0 or newer    
* Kernel headers available at compile time    
* A supported Ethernet MAC device    
* A supported PHY device paired with a MAC that allows time stamping in the PHY

* [No Hardware? Try Emulating the NIC (Slide 52)](http://events.linuxfoundation.jp/sites/events/files/slides/lcjp14_ichikawa_0.pdf)
* [The Ubuntu Forum Guide](https://ubuntuforums.org/showthread.php?t=2327884)
* [Useful Guide](http://www.elinux.org/images/f/f9/Introduction_to_IEEE_1588_Precision_Time_Protocol_%28PTP%29_Using_Embedded_Linux_Systems.pdf)

* [Configuring Apache Virtual Hosts](https://serversforhackers.com/configuring-apache-virtual-hosts)
##Some Cisco Configurations
* [Cisco Configuration and Tips (In Japanese)](http://beginners-network.com/engineer_job_change.html)
* [Configuring Trunk VLANs between Cisco Switches](http://www.networkstraining.com/how-to-configure-vlans-on-a-cisco-switch/)

