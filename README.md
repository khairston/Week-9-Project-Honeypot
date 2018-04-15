# Project 9 - Honeypot

Time spent: **6** hours spent in total

> Objective: Setup a honeypot and intercept some attempted attacks in the wild.
In this assignment, you will stand up a basic honeypot and demonstrate its effectiveness at detecting and/or collecting data about an attack. Guided instructions for doing this using specific software are provided below, but you are free to take any approach you wish that demonstrates the following basic principles:

    Successful configuration and deployment of a network-accessible honeypot server with two primary features:
        An attack surface that is vulnerable or exposed in some way to network-based attacks
        A network security feature such as an IDS configured to detect and log such attacks
    Illustration of at least one attack against the honeypot that can be detected or logged in a way that captures information about the attack or the attacker

## Honeypots deployed:
- Honeypot-1: dionaea
- Honeypot-2: snort
## Data Collected:
Number of attacks: as of 3:27PM on 04/15/2018, 71
Number of malware samples: 0

Top 5 Attacker IPs:

    191.101.167.37 (7 attacks)
    185.222.209.113 (5 attacks)
    5.188.9.25 (4 attacks)
    191.101.167.86 (4 attacks)
    123.201.150.217 (4 attacks)
    
    
Top 5 Attacked ports:

    3389 (7 times)
    445 (7 times)
    8545 (4 times)
    2000 (2 times)
    80 (2 times)


Top 5 Attacks Signatures:

    ET DROP Dshield Block Listed Source group 1 (4 times)
    ET CINS Active Threat Intelligence Poor Reputation IP TCP group 4 (2 times)
    ET CINS Active Threat Intelligence Poor Reputation IP TCP group 71 (1 times)
    ET CINS Active Threat Intelligence Poor Reputation IP TCP group 65 (1 times)
    ET CINS Active Threat Intelligence Poor Reputation IP TCP group 62 (1 times)


## Milestone 0: To the Cloud!

- [x] To complete this assignment, you'll need access to a cloud hosting provider to provision the VMs: 
<img src='Milestone-0.gif' title='Milestone 0' width='' alt='' />

## Milestone 1: Create MHN Admin VM

- [x] Start by creating the MHN Admin VM via your cloud provider: 
<img src='Milestone-1.gif' title='Milestone 1' width='' alt='' />

## Milestone 2: Install the MHN Admin Application

- [x] After having established SSH access the MHN Admin VM, the following instructions can be run on the remote VM to install the application: 
<img src='Milestone-2.gif' title='Milestone 2' width='' alt='' />

## Milestone 3: Create a MHN Honeypot VM

- [x] MHN supports multiple honeypots, each of which has a slightly different purpose you can read about. To start, we'll deploy Dionaea over HTTP, a honeypot used to trap malware samples:
<img src='Milestone-3.gif' title='Milestone 3' width='' alt='' />

## Milestone 4: Install the Honeypot Application

- [x] After having established SSH access the new honeypot VM, we need to install the honeypot application into the VM and wire it to connect back to the admin server:
<img src='Milestone-4.gif' title='Milestone 4' width='' alt='' />

## Milestone 5: Attack!

- [x] Now for the fun part: let's attack the honeypot to make sure it's all working:
<img src='Milestone-5.gif' title='Milestone 5' width='' alt='' />


## Notes

Describe any challenges encountered while doing the work

- Because I had difficulties executing the attacks with nmap, I had to reinstall the mhn admin and honeypot application.
