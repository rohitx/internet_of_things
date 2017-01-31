## Getting Started with the Internet of Things

### Introduction

IoT is a countless embedded computers, sensors, and actuators all connected online. The emergence of low-cost *microcontrollers* that are sufficiently powerful to connect to the internet. They are the key to the IoT, where all kinds of devices become the internet's interface to the physical world. 

A microcontroller (or MCU for microcontroller unit) is a small computer on a single integrated circuit. In modern terminology, it is a System on a chip or SoC. A microcontroller contains one or more CPUs (processor cores) along with memory and programmable input/output peripherals. Program memory in the form of Ferroelectric RAM, NOR flash or OTP ROM is also often included on chip, as well as a small amount of RAM. Microcontrollers are designed for embedded applications, in contrast to the microprocessors used in personal computers or other general purpose applications consisting of various discrete chips.

Microcontrollers are used in automatically controlled products and devices, such as automobile engine control systems, implantable medical devices, remote controls, office machines, appliances, power tools, toys and other embedded systems. By reducing the size and cost compared to a design that uses a separate microprocessor, memory, and input/output devices, microcontrollers make it economical to digitally control even more devices and processes. Mixed signal microcontrollers are common, integrating analog components needed to control non-digital electronic systems.

Some microcontrollers may use four-bit words and operate at frequencies as low as 4 kHz, for low power consumption (single-digit milliwatts or microwatts). They will generally have the ability to retain functionality while waiting for an event such as a button press or other interrupt; power consumption while sleeping (CPU clock and most peripherals off) may be just nanowatts, making many of them well suited for long lasting battery applications. (from Wikipedia)

Microcontrollers are cheap as they cost just $10. A hobbyist board incorporates this chip, along with Ethernet port and a Micro SD slot. The whole board costs just $60. These boards can then use sensors and actuators to interact with the physical world. Also, since the hardware allows the use of standard internet protocols, monitoring and controlling can be done over the internet.

The internet of things is a global network of computers, sensors, and actuators connected through internet protocols. Communication between a computer and a device over the internet is done using the TCP/IP protocol. While it is possible to run any kind of proprietary protocol on top of TCP/IP. However, using a standard protocol has the benefit of using many more devices as such a protocol is popular and widely available. 

### HTTP

The most important standard protocol is the `HypterText Transfer Protocol (HTTP)`. It is the protocol of the web and it describes how a client interacts with a server, by sending `request messages` and receiving `response messages` over TCP/IP. Web browsers are the most popular HTTP clients that communicate with the servers but one can write other HTTP clients and servers. 


The HTTP uses *Uniform Resource Identifiers (URIs) to tell the server which resource the client wants to read, write, create, or delete. The URIs look like the folliwng: 

* http://www.example.com/index.html
* http:///www.example.com/temperatures/actual
* http:///www.example.com/temperatures?alarm=high

A URI indicates the `scheme` (e.g. http), the `host` (e.g. www.example.com), optionally the `port` (e.g. 500000), and the `path` (e.g. /temperatures/actual) to the resource owned and managed by this host. For the HTTP protocol, port 80 is used by default unless another port is chosen explicitly. The path is called `request URI` in HTTP; it denotes the target resource of an HTTP request. 

The most popular requests a client can send are the following: 
* `GET` request for reading resource
* `PUT` for writing to a resource
* `POST` for creating a resource
* `DELETE` for deleting a resource 
