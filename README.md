# Linux_PTP_Config
General documentation and source about PTP

## Ubuntu_PTP_Config
### IEEE1588 Linux PTP

#### What is PTP
Linux PTP is a software implementation of PrecisionTime Protocol (PTP) that is in accordance with the IEEE 1588standard.  Linux PTP makes use of the Linux kernel, this allowed usto take advantage of the flexibility that is inherent to LinuxApplication Programming Interfaces (API).  Another very practicalreason for our choice was cost.  Linux PTP is free and readilyavailable for download. Some useful features of Linux PTP are as follows.

* Supports hardware and software time stamping via the Linux SO_TIMESTAMPING socket option.    
* Supports the Linux PTP Hardware Clock (PHC) subsystem by using the clock_gettime family of calls, including the new clock_adjtimex    system call.    
* Implements Boundary Clock (BC) and Ordinary Clock (OC).    
* Transport over UDP/IPv4, UDP/IPv6, and raw Ethernet (Layer 2).    
* Supports IEEE 802.1AS-2011 in the role of end station.    
* Modular design allowing painless addition of new transports and clock servos.
