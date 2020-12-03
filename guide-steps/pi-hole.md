# Title #
Setup and run Pi-Hole on a Raspberry Pi

# Summary #
Blocking ads and trackers on your devices typically requires manual labour on
each individual device (e.g. installing an ad-blocker on your browser, another
on your phone, and another on your tablet). In this guide you'll learn how to
install and setup Pi-Hole, a general purpose network-wide ad-blocker, on a
Raspberry Pi to block ads on any device connected to your home network.

# Body #

## Overview ##

Pi-hole is a general purpose network-wide ad-blocker that protects your network
from ads and trackers without requiring any setup on individual devices. It is
able to block ads on any network device (e.g. smart appliances), and, unlike
browser add-ons, Pi-hole blocks ads on any type of software.

The general setup works as follows (Fig. 1). You install Pi-hole on your server
(in this case, we're using a Raspberry Pi) and assign it a static IP address. On
your router, you set the DNS primary server to the Pi-hole IP address. When a
device connects to your home network, it gets the Pi-hole IP address as its main
DNS server from your router. When your device looks up the address for a
hostname, it contacts the Pi-hole. If the host is an ad or tracker, the request
is instantly blocked. Otherwise, the lookup is performed on some upstream server
of your choice (e.g. OpenDNS, Cloudflare, GoogleDNS, your ISP).

![Fig. 1: Pi-hole setup overview](../images/Pihole/overview.png?raw=true)

## Prerequisites ##
To deploy Pi-hole on your home network, make sure you have all of the following:

- A Raspberry Pi with at least 512MB of RAM (all Raspberry Pi versions satisfy
  this requirement) and Raspbian installed.
- An SD-card with at least 2GB of free space.
- Internet connection on your Raspberry Pi. Either via Wi-Fi (if available)
      or via Ethernet cable.
- Access to your router's administration panel[^1].

[^1]: This is standardly available in home networks. Check your router's
    documentation for instructions and credentials.

## Installation ##
If you're starting with a fresh Raspberry Pi, start by installing Raspbian
according to the [Raspberry Pi documentation][1]. Then, be sure to install `git`
with the following command:

```bash
sudo apt install git
```

To install Pi-hole, you'll clone its git repository and run the install script.

```bash
git clone --depth 1 https://github.com/pi-hole/pi-hole.git Pi-hole
cd "Pi-hole/automated install/"
sudo bash basic-install.sh
```

The script will guide you through the installation steps and ask for your input
to configure basic settings. Any settings you configure during installation can
be updated later. At some point, it asks you to select an upstream DNS provider
(Fig. 2). This is the server on which lookups of non-blocked hostnames will be
performed.

![Fig. 2: Select upstream DNS](../images/Pihole/dns.png?raw=true)

Then, it will ask you to select a couple of adlists. We suggest you leave both
on, which is the default (Fig. 3). Later, you'll be able to add custom lists if
you wish to.

![Fig. 3: Pi-hole adlist selection](../images/Pihole/adlists.png?raw=true)

Pi-hole is able to block ads on IPv4 and IPv6. Unless you have a specific reason
to disable any of those protocols, you can leave both on (Fig. 4).

![Fig. 4: Pi-hole protocol selection](../images/Pihole/protocols.png?raw=true)

It also includes a web interface which you can access to manage your Pi-hole
instance. If you're comfortable with command line usage, you can skip the web
interface (and server) installation. Otherwise, we suggest you install it (Fig.
5), as well as the corresponding web server (Fig. 6).

![Fig. 5: Install web interface](../images/Pihole/webinterface.png?raw=true)

![Fig. 6: Install web server](../images/Pihole/webserver.png?raw=true)

You can choose to log the queries answered by your Pi-hole (Fig. 7), and set a
privacy level dictating which kind of logs are stored (Fig. 8). If you're
sharing your Pi-hole instance with other people, beware that logs may leak
private information (that will be visible to you), so choose your privacy levels
accordingly.

![Fig. 7: Set query logs](../images/Pihole/logs.png?raw=true)

![Fig. 8: Set log privacy level](../images/Pihole/privacy.png?raw=true)

When the installation is finished, you'll get a summary message that includes
the IP addresses of your Pi-hole and the randomly generated admin password (Fig.
9). Be sure to save this somewhere (either screenshot or pen & paper) as you'll
need it later.

![Fig. 9: Pi-hole installation summary](../images/Pihole/summary.png?raw=true)

Click OK to conclude the installation. To be sure the installation succeeded,
open a web browser and go to <http://IP_ADDRESS/admin>, where `IP_ADDRESS` is
the IPv4 address of your Pi-hole device (Fig. 9). Note that the
<http://pihole/admin> only works **after** you setup your device to use the
Pi-hole DNS server. Click on log-in and enter your (randomly-generated)
password. You should now be in the Pi-hole admin panel (Fig. 10).

![Fig. 10: Pi-hole admin panel](../images/Pihole/admin.png?raw=true)

## Setup ##
Now that you have Pi-hole installed, the last step is configuring your network
to use Pi-hole as its DNS server

The preferred method for doing this is to change your router's DNS server and
point it to the Pi-hole IP address, ensuring any client that connects to your
network receives the Pi-hole as its DNS server. Typically this requires you to
access the router's administration panel. There, you should have a field to set
the primary and secondary DNS servers. Set the primary address to the Pi-hole's
IP address, and reset any open network connection you may have on your devices.
Now, when you connect to your home network, you should get the Pi-hole as the
DNS server.

However, some routers do not allow you to change the DNS settings. In this case,
you can set the Pi-hole as your DHCP server (and in doing so, you need to
disable your router's own DHCP server). Refer to the [official Pi-hole
documentation][2] to learn how to do so.

[1]: https://www.raspberrypi.org/software/

[2]: https://discourse.pi-hole.net/t/how-do-i-use-pi-holes-built-in-dhcp-server-and-why-would-i-want-to/3026
