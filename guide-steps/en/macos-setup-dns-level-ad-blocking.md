# Title #
Setup DNS-level ad-blocking on macOS

# Summary #
In this guide you'll learn how to manually insert DNS entries for certain types of known hosts (e.g. ad-servers, trackers, malware websites) and point them to an empty address, so that those requests are blocked on your device. Unlike browser add-ons, DNS-level ad-blocking works on *any* application or service running on your device, not just your browser. 

# Body #

DNS level content blocking prevents your device from connecting to known domains that will serve you unwanted ads and track you across all different apps and browsers on your device.

DNS or 'Domain Name System' is basically the 'phone book for the internet'. On the internet, all your requests to access websites are routed to IP addresses. Since IP addresses are sets of numbers and hard to remember, we usually address hosts by their much easier to remember host-name (e.g. privacyinternational.org).
As such, and because IP addresses can change, when your computer wants to access a server by its host-name, it asks a DNS server what the IP address for that host-name is at that moment, just like consulting a phone book, so that it can route the request correctly.
In this sense, DNS level content blocking makes use of known lists of unwanted servers - our blocklists - and purposefully give the ‘wrong address’ for domains that are on the blocklist so that your device can’t/won’t connect to those servers when it tries to.

The gold standard of protection is to set up your own pi-hole (and we have [a guide on that too](https://privacyinternational.org/guide-step/4341/raspberry-pi-setup-and-run-pi-hole)). On mobile devices, this is harder and while apps are available, their business models are still developing.

### Setup ###


To setup DNS-level ad-blocking, we will add a list of known ad-servers and trackers to the hosts file and point them to an empty address (`0.0.0.0`), thus ensuring the requests are blocked. The lists of ad-server and tracker hosts are provided and maintained by the online community, and you can pick several lists to block different types of services (e.g. ads, trackers, fake news, social media, etc.). In this guide, we suggest you use the [unified hosts list][1] from Steven Black to block ads and trackers as it is updated frequently.

Start by opening a Finder window and then navigate to the **Applications > Utilities** folder and open the **Terminal** application. Then, type the following command into the prompt:

```bash curl -o hosts.txt https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts```

and press Enter. This will download the Steven Black list to your current directory. Although unlikely, it's important to inspect the contents of the file, to ensure it does not contain malicious entries (e.g. paypal.com pointing to a phishing address that steals your credit card information). To do so, you can use `grep`. In the same terminal window, type the following command:

```bash grep -E '^(\s*)[1-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\s*.*\..*' hosts.txt```

and then press Enter. If there's any output (e.g: the command returns text) that is not for the address `127.0.0.1`, the file might have been tampered with. Delete it and choose another hosts file, for example one from [these lists][2], by clicking the corresponding link under the Original column. Replace the StevenBlack URL in the command above with this new URL. Repeat the second command to ensure that this file has not be tampered with.

If the hosts file is OK, you can move it to the correct location with the command below. On macOS, that's typically `/etc/hosts`. Please note that if you have already modified you hosts file with custom entries in the past, you need to manually merge both files (open both files on your text editor and copy-paste the appropriate contents). In the same terminal window, type the following command:

```bash cat hosts.txt | sudo tee -a /etc/hosts```

Click Enter and you will be prompted to enter your password. Write your password in the prompt (it will not show up as you type, and that's expected) and click Enter again. For the changes to have effect, you need to either restart your network services or restart your computer.

From now on, your operating system will block any request to ad-servers and trackers contained in your hosts file. To keep the hosts file up to date, periodically repeat the steps in this guide.

[1]: https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts
[2]: https://github.com/blocklistproject/Lists#lists
