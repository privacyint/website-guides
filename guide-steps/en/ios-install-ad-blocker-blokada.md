# Title #
Install an ad-blocker on iOS - Blokada

# Summary #
Blokada is a free and open-source mobile application that uses DNS servers to block ads and trackers on your device to enhance your privacy. In this guide you'll learn how to install Blokada on your iOS device.

# Body #
Blokada is an ad-blocker acting as a VPN to block unwanted traffic based on hostnames (urls). This prevents ads and malicious data from being loaded by any application running on your device.

### Installation ###

To install Blokada, visit its [Apple App Store page][1], click on **Get** (Fig. 1), and confirm by clicking **Install** when prompted (Fig. 2).

![Fig. 1: App store page for Blokada](../../images/ios/blockada-app-store.jpg?raw=true)

![Fig. 2: Install Blokada](../../images/ios/blockada-install.png?raw=true)

### Setup ###
After Blokada is installed, you can open it by clicking on the icon. By default, Blokada is disabled. To enable it, click the large button (Fig. 3).

![Fig. 3: Enable Blokada](../../images/ios/blockada-enable.jpg?raw=true)

You'll be asked to allow Blokada to setup a VPN, which is necessary to block ads. Blokada says it sets up a split-VPN, which only routes traffic on port 53, used to communicate with external DNS resolvers. What this means is that any traffic (e.g.: you trying to open privacyinternational.org in your browser) will be routed through Blokada and checked against a local DNS hostfile. If the hostname is in the list (for example an adserver), the resource won't be loaded. This prevent ads and malicious trackers and ads from being reached and displayed. 

As such, Blokada claims it **does not** monitor or filter your regular network traffic. Since it's open source and the code is publicly visible, this claim can be regularly verified. 

Click **Allow** to proceed with the setup (Fig. 4). 

![Fig. 4: Allow Blokada to setup a VPN](../../images/ios/blockada-vpn.jpg?raw=true)

Blokada should be enabled now. To select a blocking list, click on the **Advanced** tab (Fig. 5), and then select one (or more) from the list. You might want to use the same list we suggest in our DNS guides, Steven Black hosts list, as it is often updated (the first item, Energized, was last updated on 2018).

![Fig. 5: Select a blocking list](../../images/ios/blockada-lists.jpg?raw=true)

After selecting the blocking list, your device should start blocking ads immediately. To learn more about Blokada and its advanced features, visit its [official website][2].

[1]: https://apps.apple.com/us/app/blokada/id1508341781

[2]: https://blokada.org/
