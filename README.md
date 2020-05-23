### [How to Connect](#How-to-Connect) - [Meshnet DNS](#meshnet-dns) - [Adding a Peer](#adding-a-new-public-peer) - 

# DEFCONMeshNet
This meshnet is in early stages of forming. Please mind the mess!

Interesting Uses:
- Host CTF Boxes / Hosts in a fun and safe way. 
- Run Services behind firewalls and slow links
- Network is Point to Point Encrypted for your pleasure.
- Meshnet a bunch of badges together for a great time 
- Be a part of a mini, cooler internet

## How to Connect
- [Install Yggdrasil](https://yggdrasil-network.github.io/installation.html)
- Configure yggdrasil.conf
  - Linux: /etc/yggdrasil.conf
  - Windows: %PROGRAMDATA%/yggdrasil.conf
- Ensure you enable the SessionFirewall in the config, Disable AllowFromDirect, and AllowFromRemote
- Add your [closest peers](https://github.com/DEFCONMeshNet/DEFCONMeshNet/blob/master/publicnodes.csv) into the Peers section neer the top.
  - Add about 2 nearby peers.
- Review the rest of the config for settings you might like to enable. [Docs](https://yggdrasil-network.github.io/configuration.html)
- Restart Yggdrasil
- Ping ```202:7967:4d86:125c:acc1:f5bf:e719:329b``` or ```201:4771:e691:f802:373:17da:25ee:9654``` to test for connectivity.

## Meshnet DNS
The meshnet has a managed DNS server that will resolve the .defcon tld managed by this repository. All other non-mesh and all IPv4 requests will be forwarded to cloudflare 1.1.1.1 and 1.0.0.1. 

*This Name Server does not log queries in any way shape or form.*

### Usage
Set system DNS resolver to either or both:  
-```202:7967:4d86:125c:acc1:f5bf:e719:329b```  
-```201:4771:e691:f802:373:17da:25ee:9654```

### Register new Domain
Use the "New Defcon Domain Name" Issue Template to request a Domain name with the meshnet only .defcon tld.

Popular Names and exisiting groups will need reasonable proof of ownership included in the request.

## Adding a new Public Peer
You can connect to any peer on the network if you know their set listening IP and Port, It is a meshnet afterall.

If you wish to have your node publicy listed, please use the Add Public Peer issue template to register a public node.

## Known on mesh services.
To add a service, please use the Mesh Services issue template
- [DefconMeshnet Matrix](https://[200:2c03:79b4:4257:ce90:7582:4c5a:d946])
- [User.defcon self service dns bot](http://[201:6170:df3e:3de1:51a4:fac4:5b17:2d82]/)
- [Defcon Imageboard - For all your meme needs](http://[200:a8ec:216c:7550:bb88:a417:3956:d41]/index.html)
- [Defcon Hidden Wiki - For those strange things you see at linecon](http://[204:27e3:4f7c:2a89:8813:a9c6:14db:b3cc]/)

## About

Time and effort for organizing the DEFCON Meshnet and running its DNS servers have been thanks to volunteers over at DCDarknet.

## Code of Conduct

Follow the rules and guidelines set by the DEFCON Code of Conduct (CoC).

Because nodes can only connect to this network through other nodes, if you identify illegal or content against the CoC then please either disconnect/block the node from connecting to you, or report the node to be disconnected by the peer it is connected to.

Responsible Disclosure - Any vulnerabilities discovered accidentally or through allowed testing should be reported and fixed/mitigated before (if agreed to) being disclosed.

Above all, this is the DEFCON community and malicious intent should not be tolerated by its participants.
