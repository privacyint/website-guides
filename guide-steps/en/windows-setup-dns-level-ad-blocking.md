# Title #
Setup DNS-level ad-blocking on Windows

# Summary #
In this guide you'll learn how to manually insert DNS entries for certain types of known hosts (e.g. ad-servers, trackers, malware websites) and point them to an empty address, so that those requests are blocked on your device. Unlike browser add-ons, DNS-level ad-blocking works on *any* application or service running on your device, not just your browser.
# Body #

### Setup ###
In the Internet, requests are routed to IP addresses. Since IP addresses are hard to remember, we usually address hosts by their host-name (e.g privacyinternational.org). As such, and because IP addresses can change frequently, when your computer wants to access a server by its host-name, it asks a DNS server what the IP address for that host-name is, so that it can route the request. Typically, your operating systems first checks your system's *hosts file* for an address to the host-name. If the host-name is not present in the file the operating system asks an external DNS server to resolve it.

To setup DNS-level ad-blocking, we will add a list of known ad-servers and trackers to the hosts file and point them to an empty address (`0.0.0.0`), thus ensuring the requests are blocked. The lists of ad-server and tracker hosts are provided and maintained by the online community, and you can pick several lists to block different types of services (e.g. ads, trackers, fake news, social media, etc.). In this guide, we suggest you use the [MVPS hosts list][1] to block ads and trackers. We recommand this file over the Steven Black file because the format of the hosts file on Windows is different from Linux and MacOS, making the Steven Black file incompatible with Windows.

Start by downloading the `hosts.zip` file from the webpage and open it in an Explorer window. Then, select the downloaded file and click on **Extract all** (Fig. 1).

![Fig. 1: Extract hosts.zip file](../../images/Windows/hosts-extract.png?raw=true)

After the files are extracted, you might want to check the integrity of the hosts file to avoid any tempering. To do so, open a terminal window and type 

```CertUtil -hashfile C:\Users\YourUserName\pathToExtractedFile\HOSTS MD5```

The output of this command should match the one on the MVPS website (5B269EA131819DEFF186B33189C7AAD6 on 11/12/2020). If the checksum matches, right-click on the `mvps.bat` file and select **Run as administrator** (Fig. 2).

![Fig. 2: Run installer as administrator](../../images/Windows/hosts-admin.png?raw=true)

If the installer runs successfully, you should see a message reading **The MVPS hosts file is now updated** (Fig. 3).

![Fig. 3: Install notification](../../images/Windows/hosts-bat.png?raw=true)

For the changes to have effect, you need to either restart your network service, or reboot the machine. From now on, your operating system will block any request to ad-servers and trackers contained in your hosts file. To keep the hosts file up to date, periodically repeat the steps in this guide. For more information on how to manage your hosts file, check the [documentation][2] from MVPS.

[1]: https://winhelp2002.mvps.org/hosts.htm

[2]: https://winhelp2002.mvps.org/hostswin8.htm
