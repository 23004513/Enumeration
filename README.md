# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

## site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com

![Screenshot 2024-09-23 153131](https://github.com/user-attachments/assets/028acbd9-1cd6-430e-80fa-5ae4032c64b2)

## filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![Screenshot 2024-09-23 153114](https://github.com/user-attachments/assets/93b1b0ff-6d4d-4713-a743-3698576e04b5)


## intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![Screenshot 2024-09-23 153254](https://github.com/user-attachments/assets/a1a140dc-4a81-4096-a087-047e82264bce)


## inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![Screenshot 2024-09-23 153330](https://github.com/user-attachments/assets/91b63f97-4c42-4ab1-b963-c4974e784ffe)

## intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![Screenshot 2024-09-23 153432](https://github.com/user-attachments/assets/ad903811-29b5-40c0-ae19-38853e9ce871)

## link: 
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![Screenshot 2024-09-23 153504](https://github.com/user-attachments/assets/46a5588d-c3f5-4090-b3d0-d34e9cce7bd2)

## cache:
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot 2024-09-23 192015](https://github.com/user-attachments/assets/c2ebb68d-50fe-4512-9c1b-07e28c4dde64)

 
## DNS Enumeration
# DNS Recon
provides the ability to perform: Check all NS records for zone transfers Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT) Perform common SRV Record Enumeration Top level domain expansion

![Screenshot 2024-09-23 154135](https://github.com/user-attachments/assets/94979a3e-24b5-4ad2-bf1c-ea03ba1301f6)

![Screenshot 2024-09-23 154331](https://github.com/user-attachments/assets/207352be-e5da-42fc-a2b1-0b495642058f)


## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

![Screenshot 2024-09-23 154601](https://github.com/user-attachments/assets/f0995c0f-c5ea-42a4-98a2-10e7984f6882)

![Screenshot 2024-09-23 154627](https://github.com/user-attachments/assets/23c1609a-7c86-4fb5-a907-a0dbf8575603)

![Screenshot 2024-09-23 154641](https://github.com/user-attachments/assets/80486bea-f007-456e-8ac6-0fa062a74825)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/user-attachments/assets/c96f155b-0367-431d-b667-07e7745cb4ef)

select any username in the first column of the above file and check the same

![Screenshot 2024-09-23 155751](https://github.com/user-attachments/assets/8503f32f-be87-4e46-b791-76d949beb969)


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
  ![image](https://github.com/user-attachments/assets/3fbb5ce4-3d17-4b2e-8e5d-17387af587bc)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot 2024-09-23 180031](https://github.com/user-attachments/assets/bac7b855-1502-4664-bd70-b9c2cee3d1b8)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

