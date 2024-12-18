### OSI Model

How is request sent to google from PC?
How is response received back?
Journey of data (OSI Model helps us to understand it)

**Two things happens before OSI Model:**

- DNS resolution
- TCP handshake

**steps:**

- https://www.google.com =>
- => browser verify that google is mapped to any ip
- => domain name mapped with the ip address
- => if there is any mapped ip address then only move to second step (i.e TCP handshake).
- => 3 ways handshake (most popular way) is perform before OSI Model.
- => local send "Hi" to server (synk) => "synk-acknowledged" to local from server => then local send acknowledged to server.

**Only after successfull DNS resolution & TCP handshake request is made to the server**

- => browser initiates request to the server

  - http based request
  - ftp based request

    **Layer 7 -> Application Layer**

- => data encryption

  - by using https://

    **Layer 6 -> Presentation Layer**

- => session

  **Layer 5 -> Session Layer**

### Layer 7, 6 and 5 are taken care by the browser level

- => once a session is created, to transmitt data

  - data segementation/split into parts
  - protocol is defined which one to use (TCP / UDP)

    - for http it is TCP
    - for DNS it is UDP

      **Layer 4 -> Transport Layer**

- => now data is received by your router

  - for eg home router, internet service provider router etc.
  - we will source & destination ip address in each segementation. Now this segementations is known as packets.

    **Layer 3 -> Networking Layer**

- => router is connected to ethernet port or switches.

  - data is transferred to frames from packets and MAC information is also added -

          **Later 2 -> Data Link Layer**

- => It goes through multiple hobs and reaches google server.

  - again follows OCI model when it reaches google server.
  - L1 => L2 => L3 => L4 => L5 => L6 => L7

    **Layer 1 -> Physical Layer - Optical Cables( data is converted to electronic signals)**
