# Project 9 - Honeypot 

- Time spent: **8** hours spent in total

- Honeypot deployed:
    * Dionaea with HTTP
    * Shockpot
    * Snort
    * Wordpot
    * Elastichoney
## Issues Encountered
- Took some time to figure out how to utilize Google Cloud. 
  - Then create a VM instance with Compute Engine. 
- Took unfortunately a lot of time to figure out why I could not visit my page with the external ip. 
  - I had to allow http access on gcloud via the firewall and via my instance
  - [Follow this link if facing same problem](https://github.com/RedolentSun/gcloud-instructions-for-mhn/blob/master/README.md)

## Summary of the Data Collected
![1](mhn.gif?raw=true)
- What I did
  - I setup a honeypot which intentionally exposes insecure features in order to obtain information about the attacks
  - Google Cloud was used to host our server
  - We had multiple VMs, one to be the bait and the others to collect information, the actual honeypots. 
- Number of Attacks
  - 2,674
- Number of Malware Samples
  - None 
- Top 5 Attacker IPs:
  - 5.188.11.91 (80 attacks) 
  - 5.188.11.71 (73 attacks)
  - 181.214.87.34 (69 attacks)
  - 5.188.11.79 (59 attacks) 
  - 5.188.11.93 (57 attacks)
- Top 5 Attacked Ports:
  - 23 (265 times)
  - 3306 (241 times)
  - 445 (182 times)
  - 5060 (160 times)
  - 2000 (53 times)
## Unresolved Questions from Data
- We are given the date, country, sourceIP, destination port, and protocol of the attack. But this is just surface level information. 

## Note
- [json export of the data]() 

