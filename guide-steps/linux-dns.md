# Title #
Setup DNS-level ad-blocking on Linux

# Summary #

In this guide you'll learn how to manually insert invalid DNS entries for known ad-servers and trackers, so that the
requests are blocked on your device. Unlike browser add-ons, DNS-level ad-blocking works on *any* application or service
running on your device.

### Setup ###

In the Internet, requests are routed to IP addresses. Since IP addresses can change frequently, when your computer wants
to access a server by its hostname (e.g. reuters.com), it asks a DNS server what the IP address for that hostname is, so
that it can route the request. Typically, your operating systems first checks your system's *hosts file* for an address
corresponding to the hostname. Only if the hostname is not present in the file will the operating system ask a DNS
server to resolve it.

To setup DNS-level ad-blocking, we will add a list of known malicious ad-servers and trackers to the hosts file and
point them to an invalid address, to ensure requests to those hosts are blocked. These lists are provided and maintained
by the online community. You can find several list to block different types of services (e.g. ads, trackers, fake news,
social media, etc.). In this guide, we suggest you use the [unified hosts
list](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts) from Steven Black to block ads and trackers.

To download the hosts list to the correct location, open a terminal window and type:

```bash
sudo wget https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts -O /etc/
```
(Fig. 1)

Click Enter and you will be prompted to enter your password. Write your password in the prompt (it will not show up as
you type, and that's expected) and click Enter again. If nothing fails, you should now have the content of the hosts
list placed in your hosts file, which you can check by inspecting the `/etc/hosts` file in your text editor. After you
reboot your device, your operating system will block any request to malicious ad-servers and trackers contained in your
hosts file. To keep the hosts file up to date with known malicious hostnames, you should periodically run the install
command (Fig. 1). Beware that, unlike browser ad-blockers, DNS-level ad-blocking will **not** remove the ad from
webpages - it merely blocks the connection, but you will still see an empty box where the ad would be. As such,
installing a web browser ad-blocker (such as uBlock Origin) that clears the ad space from webpages is a good complement
to modifying your hosts file and provides you with a cleaner experience while browsing the web.
