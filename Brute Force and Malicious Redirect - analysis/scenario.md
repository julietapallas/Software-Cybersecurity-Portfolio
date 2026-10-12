You are a cybersecurity analyst for yummyrecipesforme.com, a website that sells recipes and cookbooks. A former employee has decided to lure users to a fake website containing malware.

The former employee/hacker carried out a brute-force attack to gain access to the web host. They repeatedly entered several known default passwords for the administrative account until they guessed the correct one. Once they obtained the login credentials, they were able to access the administration panel and modify the website's source code. They embedded a JavaScript function in the source code that prompted visitors to download and run a file when they visited the website. After embedding the malicious program, the hacker changed the administrative account password. When customers downloaded the file, they were redirected to a fake version of the website containing malware.

Several hours after the attack, multiple customers emailed the yummyrecipesforme help desk. They complained that the company's website had prompted them to download a file to access free recipes. The customers reported that, after running the file, the website address changed and their personal computers began running more slowly.

In response to this incident, the website owner attempts to access the administration panel but is unsuccessful, so they contact the website hosting provider. You and other cybersecurity analysts are assigned to investigate this security incident.

To investigate the incident, you create a sandbox environment to observe the suspicious behavior of the website. You run the network protocol analyzer tcpdump and enter the website URL, yummyrecipesforme.com. As soon as the website loads, you are prompted to download an executable file to update your browser. You accept the download and allow the file to run. You then observe that your browser redirects you to a different URL, greatrecipesforme.com, which contains the malware.

The logs show the following process:

1. The browser initiates a DNS request: It requests the IP address of yummyrecipesforme.com from the DNS server.
2. The DNS server responds with the correct IP address.
3. The browser initiates an HTTP request: It requests the yummyrecipesforme.com webpage using the IP address provided by the DNS server.
4. The browser initiates the malware download.
5. The browser initiates a DNS request for greatrecipesforme.com.
6. The DNS server responds with the IP address of greatrecipesforme.com.
7. The browser initiates an HTTP request to the IP address of greatrecipesforme.com.

A senior analyst confirms that the website has been compromised. The analyst examines the website's source code and discovers that JavaScript code has been added to prompt website visitors to download an executable file. An analysis of the downloaded file reveals a script that redirects visitors' browsers from yummyrecipesforme.com to greatrecipesforme.com.

The cybersecurity team reports that the web server was affected by a brute-force attack. The disgruntled hacker was able to guess the password easily because the administrator password was still set to the default password. In addition, there were no controls in place to prevent a brute-force attack.

Your task is to document the incident in detail, including identifying the network protocols used to establish the connection between the user and the website. You must also recommend one security measure to prevent brute-force attacks in the future.
