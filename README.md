# getDA.sh

_Disclosure: this is just a meme. Please don't actually use this._

This script checks for a few common, easy to leverage vulnerabilites I find testers using to get Domain Administrator access when stealth doesn't matter. This was a joke that turned into a POC, so please don't use this for real. It is more of a fun automation project than something actually useful.  

Currently supports:  
1. SMB relaying  
2. Kerberoasting  
3. Null session enumeration  
4. Cisco Smart Install  
5. MS17-010

I plan to add more to this as time goes on. The idea here is to provide something that you can easily throw on a Linux box inside a target network while you grab a coffee and it will spit back a few things to try.  

**Tools needed (it'll check just in case):**  
- [lgandx's fork of Responder](https://github.com/lgandx/Responder)  
- [CrackMapExec](https://github.com/byt3bl33d3r/CrackMapExec)  
- [impacket](https://github.com/CoreSecurity/impacket)  
- [SIET](https://github.com/Sab0tag3d/SIET)  
- [masscan](https://github.com/robertdavidgraham/masscan)  
- [rpcclient](https://www.samba.org/samba/docs/man/manpages-3/rpcclient.1.html)  
- [nmap](https://nmap.org/)  
- [type7decrypt.pl](https://github.com/matterpreter/misc/blob/master/type7decrypt.pl)  
  
*ALL AUTOPWN FEATURES ARE UNTESTED AND EXPERIMENTAL!*

**To Do:**
- [x] MS17-010
- [x] Test MS17-010
- [x] Fix MS17-010 scan result parser
- [x] Complete null session tests
- [ ] Implement SMB message signing checks as their own function
- [ ] Automatic scope generation
- [ ] Autopwn? :)
