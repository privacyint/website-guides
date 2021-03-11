# Title  #
Install a CDN-emulator on Chrome (and derivatives) - Decentraleyes

# Summary #
Decentraleyes is a browser add-on used for local content delivery network (CDN) emulation, that protects your privacy by evading large CDNs (e.g. Google Hosted Libraries). In this guide, you'll learn how to install Decentraleyes on Chrome (and derivatives) to prevent CDNs from tracking your online activity.

# Body #
Content delivery networks (CDNs) are geographically distributed network of proxy servers that seek to provide features such as better availability and performances for websites. While the goal is commendable, it also means that these CDN providers receive metadata related to the websites you visit (where they are setup). With this is mind, you might want to sacrifice the added convenience and avoid large CDN providers (such as Google and Cloudfare) to prevent them from obtaining any data related to your online browsing.

To do so, this guide will explain how to install Decentraleyes on Chrome (and derivatives).

### Installation ###

Like any other add-on, install Decentraleyes by visiting the [Chrome Web Store][1] and clicking **Add to Chrome** (Fig. 1) and then clicking on **Add extension** when prompted (Fig. 2).

![Fig. 1: Download Decentraleyes](../images/Chrome/decentraleyes-add.png?raw=true)

![Fig. 2: Add Decentraleyes to Chrome](../images/Chrome/decentraleyes-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../images/Chrome/decentraleyes-notify.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the Decentraleyes icon is added to the extension menu on your toolbar (Fig. 3). To pin the icon on the toolbar, click the extension menu, and then click the pin next to the Decentraleyes icon. When you visit a website, Decentraleyes automatically blocks connections to third-party CDNs and injects the assets locally, which you can check by clicking the icon (Fig. 4).

![Fig. 4: Decentraleyes pop-up interface](../images/Chrome/decentraleyes-test.png?raw=true)

You can test the add-on by visiting the [Decentraleyes testing utility][2]. If you are interested in more advanced usage, visit the [official documentation page][3].

[1]: https://chrome.google.com/webstore/detail/decentraleyes/ldpochfccmkkmhdbclfhpagapcfdljkj

[2]: https://decentraleyes.org/test/

[3]: https://git.synz.io/Synzvato/decentraleyes/-/wikis/
