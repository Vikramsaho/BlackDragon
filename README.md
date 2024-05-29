# BlackDragon
The Web Hacking Advance Automated tool.


Skip to content
Navigation Menu
Aleph-works
/
BlackDragon-web-recon-automation-tool-Linux

Type / to search

Code
Pull requests
Actions
Projects
Security
Insights
Owner avatar
BlackDragon-web-recon-automation-tool-Linux
Public
forked from sniper199/BlackDragon
Aleph-works/BlackDragon-web-recon-automation-tool-Linux
Go to file
t
Add file
This branch is 17 commits ahead of, 30 commits behind sniper199/BlackDragon:main.
Folders and files
Name		
Latest commit
Cyber-Guy1
Cyber-Guy1
Fixing gobuster #2
63c07f5
 · 
3 years ago
History
nuclei-templates
uploading nuclei temps
3 years ago
Black-Dragon
Fixing gobuster #2
3 years ago
BlackDragon - Recon.pdf
Add files via upload
3 years ago
BlackDragon - Recon.png
Add files via upload
3 years ago
LICENSE.md
Add files via upload
3 years ago
README.md
Update README.md
3 years ago
VIPX.png
Add files via upload
3 years ago
gplv3-with-text-136x68.png
Add files via upload
3 years ago
install
Update install
3 years ago
Repository files navigation
README
License
Black-Dragon V2.0 [VIPX Edition]
An Advanced Automation Tool For Web-Recon Developed For Linux Systems


What Is Black Dragon ?
It's A Tool To Automate The Web Reconnaissance Proccess, Which Make It Easier To Gather Informations About Your Target. This Tool Will Help You In Your Bug Hunting Or Web Penetration Testing Operation Because It Not Only Gather Informations About The Target, But Also It Arranges All These Information In A Structed Way Which Makes You Analyse The Data In A Good Way.

This Tool Works In Linux Systems, Specially In Debian & Debian Based Systems.

Tested On:

Kali Linux
Parrot OS
Back Box
And Other Debian Based Linux Distro's

What Is The Best Use For This Tool ?
This Is An Automated Tool, So Simply You Give It A Target Then Simply The Tool Took All The Information & And Save The Results In Ordered Directories & Files, But When You Do The Recon You Just Use This Tool, But Also You Should Do Some Manual Activity, This Mindmap Shows The Whole Operation Of BlackDragon Recon Methodology:


So Any Tool Based Recon In This Methodology, I Put It Here In This Automation Tool, But I Prefer To Do So Recon Manually, So First You Should Search Deeply In The IOT Search Engines Like:

 Shodan.io
 Censys.io
 Zoomeye
Also You Should Search In Some FTP Search Engines Like:

 SearchFTPs
 Search Archive
 File Searching
 Free Ware Web
 MMNT.ru
 FTP Sites
When You Wanna Make A Powerfull Recon, You Should Also Look At:

 Hunter.io -> For Target Email Searching
 Public-WWW -> For String Searching In Public Source Codes
What Did This Tool Do:
Subdomain-Gathering Using:

 Subfinder

 Sublist3r

 Amass

Enum:

Active Recon
Passive Recon
Intel:

Active Recon
 Assetfinder

 Knockpy

 github-subdomains

Getting The Whole Subdomain Gathered Then Filter The Unique Domains And Extract The Only Live Subdomain Using:

 httpx

Fuzzing The Application Target Based Using:

 Gobuster

 Dirsearch

 Dirb

Endpoints Gathering Using:

 Waybackurls

 github-endpoints

DNS Information Gathering Using:

 DNSMap

 DNSEnum

 MassDNS

 Gobuster

Port Scanning

 rustscan

What's New In This Version [2.0] ?
Bug Fixes

Amass Enum Passive & Active Recon

Amass Intel Passive & Active Recon

Domains Ports Discovery & Screen Shootig

Vulnerability Scanning:

CVE Scanning
Workflow Scanning
Default-Logins Scanning
Takeovers Scanning
Exposed Panels Scanning
IoT Search Engine Recon [Shodan]:

Domain Info Gathering
Host Info Gathering
Honeypot Checker
HTTP & HTTPS Filtering

Smarter Functionalities

Installation
Be Sure To Delete The Previous Version The Install The New
First Delete The Previous Version If Exists:

rm -rf BlackDragon

Then Simply After Cloning The Repository By Typing :

git clone https://github.com/Vikramsaho/BlackDragon.git

Then Open Up The BlackDragon Directory:

cd BlackDragon/

After That Give The Execution Permission To The Installation Script And The Tool Script:

chmod +x install; chmod +x Black-Dragon

Finally Run The Installation Script:

./install

Tool Using Syntax:
Simply:

./Black-Dragon example.com

Note: DO NOT Add http:// or https:// In The Domain, The Tool Do This Automatically

Tool Output Example
cyber-guy@Security:~/BlackDragon$ ./Black-Dragon google.com

                                         `.-:/+oosssoo+/::-.
                                    `:oydmNNMMMMMMMMMMMMMNNNmdyo/-`
                                   -dNMMMMMMMMMMMMMMMMMMMMMMMMMMMNmh+-`
                                    ........-:/oydNMMMMMMMMMMMMMMMMMMNms:`
                                           .:os  `.yMMMMMMMMMMMMMMMMMMMMNd+`
                                         :ymMm/ ``.oMMMMMMMMMMMMMMMMMMMMMMMm/
                                   ..++yhNMMMmmmmmmMMMMMMMMMMMMMMMMMMMMMMMMMMh.
                                `/ymNMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMs:omd.
                              .smMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM/  `+y`
                             /NdoyMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMN/   .-
                            `NMddNMMMMMMNmNMddddmNNMMMMMMMMMMMMMMMMMMMMMMMMMy-
                            `oddddhyso/-.`.-` ```.-:ohNMMMMMMMMMMMMMMMMMMMMMMNy-
                              ```     ``..            .+dMMMMMMMMMMMMMMMMMMMMMMNo
                                  ./ohdmmo```..         `/mMMMMMMMMMMMMMMMMMMMMMMs
                               .+hNMMMMMMNmmmmm:.....`    .dMMMMMMMMMMMMMMMMMMMMMM-
                             `omMMNNmmmNNMMMMMMMNmmm+-.    `mMMMMMMMMMMMMMMMMN+:yM/
                            `hMmy/-.....-:/ohmNMMMMo        +MMMMMMMMMMMMMMMMh  `m`
                            sMd.             `-sNMMs        -MMMMMMMMMMMMMMMMs  ..
                            NM+                 .yMN        +MMMMMMMMMMMMMMMM/
                            NMh`                 `hm       .mMMMMMMMMMMMMMMMm`
                            sMMy.                 --      :mMMMMMMMMMMMMMMMM/
                            `dMMNs-`                   `:yMMMMMMMMMMdymMMMN+
                             .hMMMMds/-.`         `.-+ymMMMMMMMMMMNo` hMMm:
                               +mMMMMMMNdhyysssyyhdNMMMMMMMMMMMMms.  +Mmo`
                                `/ymMMMMMMMMMMMMMMMMMMMMMMMMNmh/`   +s:`
                                   `:ohmNNMMMMMMMMMMMMNNNdy+:`
                                        .-:/+osssso++/:.`

			          An Automated Tool For Web-Recon
					Developed By Momen Ali
					    The CyberGuy
						v-2.0

                                         _    __________ _  __
                                        | |  / /  _/ __ | |/ /
                                        | | / // // /_/ |   / 
                                        | |/ _/ // ____/   |  
                                        |___/___/_/   /_/|_|  
                      


====================================
               Banner                  
====================================

[+] Target Domain => google.com
[+] Date => 05-05-2021
[+] Current User => cyber-guy

-------------------------------------

[+] Current Recon Path: => /home/Vikramsaho/BlackDragon/google.com/05-05-2021

====================================

Stay Secure ;)

GPL V3 License


About
An Adavnced Automation Tool For Web-Recon Developed For Linux Systems

Resources
 Readme
License
 GPL-3.0 license
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 0 forks
Report repository
Releases
 2 tags
Packages
No packages published
Languages
Shell
98.9%
 
Python
1.1%
Footer
© 2024 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact
Manage cookies
Do not share my personal information
