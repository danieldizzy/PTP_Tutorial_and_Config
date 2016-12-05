
## First What is TSN 
This standard is one of a number of IEEE 802.1 and other standards suitable for Time-Sensitive Networking
(TSN) that together have the overall goal of providing extremely low packet loss rates and finite, low, and
stable end-to-end latencies. TSN supports unicast and multicast Streams of packets that implement a wide
range of demanding real-time applications including audio/video studios, industrial processes, and the
control of machines and vehicles. The TSN goals are not achieved at the expense of hampering the ability of
the network to carry traffic for non-time-critical applications.

## Linux PTP Config
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

## To read for Research
* [Using an NFC-equipped mobile phone as
a token in physical access contro](essay.utwente.nl/65419/1/thesis_nfc_martijn_bolhuis_final.pdf)
* [Context Aware Healthcare System](http://www.ijimt.org/papers/432-D0142.pdf)
* [Context Awareness in healthcare](http://www3.nd.edu/~cpoellab/teaching/cse40816/papers/TD05.pdf)
* Consider a research topic in using PTP for healthcare based context ware systems, In current context aware systems a key aspect user to determine the context is the date and time. However, Current systems use NTP services for providing the context aware systems. which is succeptable to security attacks just like any other computer node on the network. So we propose the use of Hard ware based time synchronization for context aware systems where instead of depending on NTP we depend emply the use of hardware time stamping in based on PTP protocol. 
  * Modern healthcare networks will be performing remote services and some of these systems are sychronized together. 
  * Which some also depend on time synchonization for services. like monitoring patients health status at timely intervals.
  * Using it as secure alarm systems to raise alarms based on some change in context.
  * The can be cheaper as compared to managing NTP because they are handled on layer Network Layer whislt the NTP operates on the Application layer. From a security stand point this may be necessary to investigate.
  * **Steps to evaluate the use case :**
      * Obtain beagle bones to simulate the PTP protocol and the NTP protocol.
      * Do a performance evaluation from the PTP protocol and compare the results based on the data collected 
      * Bulid an attack scenario of the NTP server being hacked and time changed and that of the PTP time not being changed on a system 
      * Since PTP is mainly applied in connected bridges it will be best if you consider a scenario with multiple networks in a hospital syste. 
      * perform your discussions and data visualizations for each test and conclude the paper.

* **Some Referece Sources**:
* [Source about TSN ](https://www.odva.org/Portals/0/Library/Conference/2015_ODVA_Conference_Ditzel-Didier_TSN.pdf)
* [Source about PTP and TSN](https://www.eecis.udel.edu/~mills/ptp.html)

## OPC-UA Pub/Sub

* [Pub-Sub Security](http://www.opcfoundation.org/UA/Part2/)
* [Introduction to OPC-UA](http://home.hit.no/~hansha/documents/control/opc/OPC%20Overview.pdf)
* [Babbling Idiots Problem](http://www.ieee802.org/1/files/public/docs2013/new-tsn-jochim-ingress-policing-1113-v1.pdf)

## Presentation Guide
* [Oral Presentation Structure](http://www.nature.com/scitable/topicpage/oral-presentation-structure-13900387)
