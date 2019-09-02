# CVE-2019-11510
Exploit for Arbitrary File Read on Pulse Secure SSL VPN (CVE-2019-11510)

You can use a single domain, either a list of domains. You must include https:// in front of the domain.

Usage : cat targetlist.txt | bash CVE-2019-11510.sh / bash CVE-2019-11510.sh -d https://vpn.target.com/

If you want to just verify the exploit and download /etc/passwd then use :  

cat targetlist.txt | bash CVE-2019-11510.sh --only-etc-passwd

bash CVE-2019-11510.sh -d https://vpn.target.com/ --only-etc-passwd

Output will be saved inside output/vpn.target.com/

Demo : 

![CVE-2019-11510.sh demo](https://github.com/projectzeroindia/CVE-2019-11510/raw/master/CVE-2019-11510.PNG)


Reference/Credits
---

https://blog.orange.tw/2019/09/attacking-ssl-vpn-part-3-golden-pulse-secure-rce-chain.html

https://www.blackhat.com/us-19/briefings/schedule/index.html#infiltrating-corporate-intranet-like-nsa---pre-auth-rce-on-leading-ssl-vpns-15545

https://blog.orange.tw/2019/08/attacking-ssl-vpn-part-2-breaking-the-fortigate-ssl-vpn.html

https://i.blackhat.com/USA-19/Wednesday/us-19-Tsai-Infiltrating-Corporate-Intranet-Like-NSA.pdf
