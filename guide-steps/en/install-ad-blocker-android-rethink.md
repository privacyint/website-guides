# Title #
Install an ad-blocker on Android - Rethink

# Summary #
Rethink is a free and [open-source](3) mobile application that uses DNS servers to block ads and trackers on your device to enhance your privacy. In this guide you'll learn how to install Rethink on your Android device.

# Body #
Rethink is an ad-blocker that uses DNS servers to block malware, spyware, ads, and trackers across all apps on your device based on their hostname (URL). It also allows you to setup a firewall and a proxy for your connections. In this guide, you will learn how to use Rethink to setup DNS-level ad-blocking to block ads and trackers across your mobile apps and browser.

### Installation ###

To install Rethink, visit its [Play Store page][1] and click on **Install** (Fig. 1).

![Fig. 1: Play store page for Rethink](../../images/Android/rethink-install.png?raw=true)

### Setup ###

After Rethink is installed, you can open it by clicking on the icon or clicking on **Open** in the Play Store. By default, Rethink is configured to setup both DNS and Firewall. In order to block ads, it is enough to setup DNS. Unless you have a specific need for a firewall, we suggest you leave it off, as this may unintentionally block regular traffic on your device, which may affect your browsing experience or Internet-connect apps. To change the default mode, click the arrow next to the **Start** button (Fig. 2) and then choose the first option, **DNS** (Fig. 3). To enable Rethink, click the **Start** button.

![Fig. 2: Enable Rethink.](../../images/Android/rethink-open.jpg?raw=true)

![Fig. 3: Configure default Rethink modes.](../../images/Android/rethink-modes.jpg?raw=true)

Once Rethink is running, it will route all DNS requests performed by your device (even in apps) through a DNS server of your choosing, and show you an overview of its activity (Fig. 4). It also allows you to setup blocklists for specific hostnames you want to block. This means that, if an app tries to track you by sending your data to the hostname `evil-tracker.org`, you can block the hostname in Rethink and the app is unable to send data (since the host can not be found), effectively protecting your device against this form of digital tracking.

![Fig. 4: Rethink screen when running.](../../images/Android/rethink-working.jpg?raw=true)


To configure the DNS settings, click the **DNS** card in the main screen. In this page (Fig. 5), you can change the DNS server (i.e. the one answering requests from your device), and configure blocklists you want to use.

![Fig. 5: Rethink DNS settings.](../../images/Android/rethink-dns-settings.jpg?raw=true)

To configure blocklists, which are disabled by default, click the **On-device blocklists** option and then click on **Disabled**. This will prompt you to download blocklists that you can later enable. Click on **Download blocklists** to proceed. After the download finishes, you are shown a screen with categorized blocklists. To find privacy-related lists, scroll down to the **Privacy** section. We suggest you enable, at least, the **Recommended** lists. Finally, click **Apply** to save your changes.

![Fig. 6: Rethink privacy blocklists.](../../images/Android/rethink-blocklists.jpg?raw=true)

After enabling blocklists, your device should start blocking ads and trackers immediately. You can check this in the home screen of Rethink, in the **Apps** card (Fig. 2). To learn more about Rethink and its advanced features, visit its [official website][2].

[1]: https://play.google.com/store/apps/details?id=com.celzero.bravedns
[2]: https://rethinkdns.org/
[3]: https://github.com/celzero/rethink-app