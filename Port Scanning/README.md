# Port Scanning using Nmap

## What is Nmap?

Nmap is a short form of Network Mapper and it’s an open-source tool that is used for mapping networks, auditing and security scanning of the networks. The reason behind its development is to quickly find large networks at a specific location. For the discovery of networks, the raw IP packets are used by Nmap. The most common use of Nmap is for security audits of networks.

## Nmap Commands

**Scan a Range of IP Address** : To scan a range of IP addresses, the Nmap command is as follows:

    nmap (ip address)
**Speed up Scan of IP Address** : To scan a range of IP addresses at a faster rate, the Nmap command is as follows:

    nmap -F (ip address)
**Scan a Port of IP Address** :  To scan a specified port or mulitiple port of IP addresses, the Nmap command is as follows:

    nmap -p (ip address)
     nmap -p p1,p2,p3 (ip address)
**Scan a Range based Port of IP Address** :  To scan a Range of port specified in a IP addresses, the Nmap command is as follows:

    nmap -p p1-pn (ip address)
**Scannig based on service of IP Address** :  To scan a Range of port based on service they provide in a IP addresses, the Nmap command is as follows:

    nmap -p mysql,https,ftp (ip address)
**Service Version Detection** : The service version can be detected for IPv4 script with the help of Nmap by using following command:

    nmap -A (ip address)
**Output Formats** :  To save default output to a file by using following command:

    nmap -oN (filename.txt) (ip address)
**NSE scripts** : To get more information about NSE scripts and scan some default scripts, the Nmap command is as follows:

    nmap -sV -sC (ip address)
