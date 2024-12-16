## Networking Concepts:

### IP Address:

- generate/provide unique address to a particular device that is connected to the local network.
- IPV4 / IPV6
- eg IPV4: 172.16.3.4 or 10.1.2.4
- each number i IP address can vary from `0-255`
- each number is 1 byte -> 8 bits
- four numbers = 4 bytes -> 32 bits
- all four numbers are separeted by dots(.)
- DNS for www.google.com is 8.8.8.8

### convert given IP (172.32.16.1) into bits format:

- 172 => 2*7 + 2*5 + 2*3 + 2*2
- 32 => 2\*5
- 16 => 2\*4
- 1 => 2\*0

### Subnet: Sub-networking also known as CIDR range

- dividing a network into sub parts.
- benefits: security, privacy & isolation.
- 172.16.3.0/24 CIDR range for subnet
- 32-24=8 => 2\*8=> 256 ip addresses
- 32-31= 1 => 2\*1 => 2 ip addresses

### Subnet => private & public subnet

- **private subnet:** doesn't have access to internet.
- **public subnet:** have access to internet.

### For ex: public subnets

- /27 means 32-27 = 5 => 2\*5= 32 ip addresses
- /28 means 32-28 = 4 => 2\*4= 16 ip addresses
- /29 means 32-29 = 3 => 2\*3= 8 ip addresses

### For ex: private subnets

- 192
- 172
- 10

### Ports

- for ex. :9191
- when ever we host a application on VM. To access the application via internet we need two things:
  - IP address of VM (public) 3.4.5.6
  - port :5162
  - for ex. 3.4.5.6:5162
