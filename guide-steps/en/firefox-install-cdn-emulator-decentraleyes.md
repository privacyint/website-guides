*Currently visible at:https://privacyinternational.org/node/4321*

# Title  #
Install a CDN-emulator on Firefox 

# Summary #
Using a local content delivery network (CDN) emulation can help protect your privacy by evading large CDNs (e.g. Google Hosted Libraries). In this guide, you'll learn how to install a CDN emulator on Chrome (and derivatives) to prevent CDNs from tracking your online activity.

# Body #
Content delivery networks (CDNs) are geographically distributed network of proxy servers that seek to provide features such as better availability and performances for websites. While the goal is commendable, it also means that these CDN providers receive metadata related to the websites you visit (where they are setup). With this is mind, you might want to sacrifice the added convenience and avoid large CDN providers (such as Google and Cloudflare) to prevent them from obtaining any data related to your online browsing. You can read more about the risks of using public CDNs [here](https://httptoolkit.com/blog/public-cdn-risks/)

To avoid large CDN providers you can use tools such as Decentraleyes, an [open source](https://git.synz.io/Synzvato/decentraleyes) extension that we'll go through bellow. 


### Installation ###
Like any other add-on, install Decentraleyes by visiting the [Mozilla Firefox Add-ons page][1] and clicking **Add to Firefox** (Fig. 1) and then clicking on **Add** when prompted (Fig. 2).

![Fig. 1: Download Decentraleyes](../../images/Firefox/decentraleyes-add.png?raw=true)

![Fig. 2: Add Decentraleyes to Firefox](../../images/Firefox/decentraleyes-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../../images/Firefox/decentraleyes-notify.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the Decentraleyes icon is added to your toolbar (Fig. 3). When you visit a website, Decentraleyes automatically blocks connections to third-party CDNs and injects the assets locally, which you can check by clicking the icon (Fig. 4).

![Fig. 4: Decentraleyes pop-up interface](../../images/Firefox/decentraleyes-test.png?raw=true)

You can test the add-on is working correctly by visiting the [Decentraleyes testing utility][2]. If you are interested in more advanced usage, visit the [official documentation page][3].

[1]: https://addons.mozilla.org/en-US/firefox/addon/decentraleyes/

[2]: https://decentraleyes.org/test/

[3]: https://git.synz.io/Synzvato/decentraleyes/-/wikis/
