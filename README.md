# computer_networks
_Understand the various network layer, transport layer and application layer protocols and it also helps to design and implement the protocols using socket programming._

## Topics covered
=> Necessary header files with respect to socket programming. </br>
=> Basic Functions of Socket Programming. </br>
=> Simple TCP/IP Client Server Communication. </br>
=> UDP Echo Client Server Communication. </br>
=> Concurrent TCP/IP Day-Time Server. </br>
=> Half Duplex Chat Using TCP/IP. </br>
=> Full Duplex Chat Using TCP/IP. </br>
=> Implementation of File Transfer Protocol. </br>
=> Remote Command Execution Using UDP. </br>
=> Arp Implementation Using UDP. </br>

## Using the repository
Test using ```./server``` in a terminal separately and ```./client``` in a different terminal.

## Header Files
The header files with respect to Socket Programming

### ```stdio.h```
It is standard input and output library that provides simple and efficient buffered stream for IO interface.(scanf, printf, gets, putc etc.)

### ```unistd.h```
It is a POSIX [Portable Operating System Interface] standard for open system interface. (fork, pipe, read, write etc.)

### ```string.h```
This header file is used to perform string manipulation operations on NULL terminated strings.(strcpy,strcmp, strlen etc.)

### ```stdlib.h```
This header file contains the utility functions such as string conversion routines, memory allocation routines, random number generator, etc. (abort, exit, rand, atoi etc.)

### ```sys/types.h```
This header files defines the data type of socket address structure in unsigned long.( clock_t, size_t, dev_t etc.)

### ```sys/socket.h```
The socket functions can be defined as taking pointers to the generic socket address structure called sockaddr. (SO_REUSEADDR, SO_ERROR, SO_ACCEPTCONN etc.)

### ```netinet/in.h```
This defines the IPv4 socket address structure commonly called Internet socket address structure called sockaddr_in. (IPPROTO_IP, IPPROTO_ICMP, IPPROTO_TCP etc.)

### ```netdb.h```
This defines the structure hostent for using the system call gethostbyname to get the network host entry. (HOST_NOT_FOUND, NO_DATA, NO_RECOVERY etc.)

### ```time.h```
It has structures and functions to get the system date and time and to perform time manipulation functions. We use the function ctime() that is defined in this header file to calculate the current date and time.

### ```sys/stat.h```
It contains the structure stat to test a descriptor to see if it is of a specified type. Also it is used to display file or file system status.stat() updates any time related fields. When copying from 1 file to another.

### ```sys/ioctl.h```
Macros and defines used in specifying an ioctl request are located in this header file. We use the function ioctl() that is defined in this header file. ioctl() function is used to perform ARP cache operations.

### ```pcap.h```
It has function definitions that are required for packet capturing. Some of the functions are pcap_lookupdev(),pcap_open_live() and pcap_loop(). pcap_lookupdev() is used to initialize the network device. The device to be sniffed is opened using the pcap_open_live(). pcap_loop() determines the number of packets to be sniffed.

### ```net/if_arp.h```
It contains the definitions for Address Resolution Protocol. We use this to manipulate the ARP request structure and its data members arp_pa,arp_dev and arp_ha. The arp_ha structure’s data member sa_data[ ] has the hardware address.

### ```errno.h```
It sets an error number when an error and that error can be displayed using perror function. It has symbolic error names. The error number is never set to zero by any library function.

### ```arpa/inet.h```
This is used to convert internet addresses between ASCII strings and network byte ordered binary values (values that are stored in socket address structures). It is used for inet_aton, inet_addr, inet_ntoa functions
