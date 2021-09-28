## Reconky-Automated Bash Script

```---------	 _______  _______  _______  _______  _        _                
(  ____ )(  ____ \(  ____ \(  ___  )( (    /|| \    /\|\     /|
| (    )|| (    \/| (    \/| (   ) ||  \  ( ||  \  / /( \   / )
| (____)|| (__    | |      | |   | ||   \ | ||  (_/ /  \ (_) / 
|     __)|  __)   | |      | |   | || (\ \) ||   _ (    \   /  
| (\ (   | (      | |      | |   | || | \   ||  ( \ \    ) (   
| ) \ \__| (____/\| (____/\| (___) || )  \  ||  /  \ \   | |   
|/   \__/(_______/(_______/(_______)|/    )_)|_/    \/   \_/   
``` 

# About

Last time Tested 27th September of 2021 on Kali Linux 2021.3

Reconky is a script written in bash to automate the task of recon and information gathering. This Bash Script allows you to collect some information that will help you identify what to do next and where to look for the required target.

# Main-Features

- It will Gathers Subdomains with assetfinder and Sublist3r
- Duplex check for subdomains using amass
- Enumerates subdomains on a target domain through dictionary attack using knockpy
- searchs for alive domains using Httprobe
- Investigates for feasible subdomain takeover
- Scans for open ports using nmap
- Pulls and Assembls all possible parameters found in wayback_url data
- Pulls and compilis json/js/php/aspx/ files from wayback output
- Runs eyewitness against all the compiled(alive) domains


# Install pre-requisites as root

```ShellSession
sudo -i
```

1. [Sublist3r](https://github.com/4k4xs4pH1r3/Sublist3r)
2. [Amass](https://github.com/4k4xs4pH1r3/Amass)


# Install Reconky as root
```ShellSession
sudo -i
```

```ShellSession
cd /usr/share/ && git clone https://github.com/ShivamRai2003/Reconky-Automated_Bash_Script.git && cd Reconky-Automated_Bash_Script && chmod +x install.sh reconky.sh && ./install.sh
```

# Usage as root
```ShellSession
sudo ./reconky.sh yourdomain.com
```


# DEMO
![cli output](https://github.com/ShivamRai2003/Reconky-Automated_Bash_Script/blob/main/Recon.gif)

# Authors and Thanks

`This script makes use of tools developped by the following people`
- Cyber Mentor 
- Tom Hudson - Tomonomnom
- OWASP
- Ahmed Aboul-Ela - Aboul3la
- Gianni Amato
- FortyNorth Security
- Gordon Lyon

`Note : If install.sh does not complete the pre-requisites, kindly install all the tools manually described in that. So that directory problem will not occur and make sure all the tools can be run globally from any directory for that use symbolic link.`

### Happy Hunting
`Note : Run with Caution. Pull Request and New Ideas Is Welcome. `
