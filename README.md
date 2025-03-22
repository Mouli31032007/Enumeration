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

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![shot 1](https://github.com/user-attachments/assets/a5db466e-df09-46e0-81e3-3adcfffb2162)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![shot 2](https://github.com/user-attachments/assets/a5c80368-163d-46f6-8a2d-f05fcaa9cac8)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![shot 3](https://github.com/user-attachments/assets/0e9580be-25d2-45ee-9747-febc0ac5b3ab)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![shot 4](https://github.com/user-attachments/assets/32f8b27a-fff6-478d-9b36-60059714d0f9)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![shot 5](https://github.com/user-attachments/assets/6ece4c4b-8cf1-4215-9ad6-936b444ac451)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![shot 6](https://github.com/user-attachments/assets/bc7568cf-c2f9-42da-8b2f-a32ccbd79a94)

 
#DNS Enumeration
![shot 7](https://github.com/user-attachments/assets/7515de30-c947-4059-8a29-83736942963f)


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![shot 8](https://github.com/user-attachments/assets/7adb0b38-4d08-4b02-bdaf-23e11890d54a)



##dnsenum
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
![shot 9](https://github.com/user-attachments/assets/225dd50d-e5c2-497e-8abc-1d96e02a84a8)
#smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![shot 10](https://github.com/user-attachments/assets/c6d8a6d2-e13f-4eed-81a2-4810f761669c)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![shot 11](https://github.com/user-attachments/assets/5ebdf206-775a-460c-9b9b-b3409b40fdf0)

select any username in the first column of the above file and check the same
![shot 12](https://github.com/user-attachments/assets/aacc780b-db58-461d-92d9-52825813db36)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

![shot 13](https://github.com/user-attachments/assets/702c1671-cf86-4307-86fa-0254ce9749c9)

# nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![shot 14](https://github.com/user-attachments/assets/298ffd2d-d5e2-413e-84e7-6faa8ef0cf08)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![image](https://github.com/user-attachments/assets/d92dec8e-0254-48f9-8fea-f6666bc305a9)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

