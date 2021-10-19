# Title #
Setup DNS-level ad-blocking on Linux

# Summary #
In this guide you'll learn how to manually insert DNS entries for certain types of known hosts (e.g. ad-servers, trackers, malware websites) and point them to an empty address, so that those requests are blocked on your device. Unlike browser add-ons, DNS-level ad-blocking works on *any* application or service running on your device, not just your browser. 

# Body #

### Setup ###
On the Internet, requests to access websites are routed to IP addresses. Since IP addresses are hard to remember, we usually address hosts by their host-name (e.g. privacyinternational.org). As such, and because IP addresses can change frequently, when your computer wants to access a server by its host-name, it asks a DNS server what the IP address for that host-name is, so that it can route the request. Typically, your operating system first checks your system's *hosts file* for an address to the host-name. If the host-name is not present in the file, the operating system asks an external DNS server to resolve it.

To setup DNS-level ad-blocking, we will add a list of known ad-servers and trackers to the hosts file and point them to an empty address (`0.0.0.0`), thus ensuring the requests are blocked. The lists of ad-server and tracker hosts are provided and maintained by the online community, and you can pick several lists to block different types of services (e.g. ads, trackers, fake news, social media, etc.). In this guide, we suggest you use the [unified hosts list][1] from Steven Black to block ads and trackers as it is updated frequently.

To download the hosts list, open a terminal window and type the following command

```wget https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts -O hosts ```

and then press Enter. The file will be downloaded to your current directory. Although unlikely, it's important to inspect the contents of the file, to ensure it does not contain malicious entries (e.g. paypal.com pointing to a phishing address that steals your credit card information). To do so, you can use `grep`. In the same terminal window, type the following command

```grep -E '^(\s*)[1-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\s*.*\..*' hosts ```

and then press Enter. If there's any output (e.g: the command returns text), the file might have been tampered with. Delete it and choose another hosts file, for [example from this list](https://github.com/EnergizedProtection/block#formats). Once you have the URL for the this new list (for example the blu list URL is https://block.energized.pro/blu/formats/hosts.txt), replace the StevenBlack URL in the command above with this new URL. Repeat the second command to ensure that this file has not be tempered with.

If the hosts file is OK, you can move it to the correct location. On Linux systems that's typically `/etc/hosts`, but be sure to check your distribution's manual. Please note that if you have already modified you hosts file with custom entries in the past, you need to manually merge both files (open both files on your text editor and copy-paste the appropriate contents). In the same terminal window, type the following command.

```sudo mv hosts /etc ```

Click Enter and you will be prompted to enter your password. Write your password in the prompt (it will not show up as you type, and that's expected) and click Enter again. For the changes to have effect, you need to either restart your network service (check your distribution's manual for instructions on how to do that), or reboot the machine.

From now on, your operating system will block any request to ad-servers and trackers contained in your hosts file. To keep the hosts file up to date, periodically repeat the steps in this guide.

[1]: https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts
