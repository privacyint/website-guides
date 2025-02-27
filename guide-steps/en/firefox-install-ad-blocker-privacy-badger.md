*Currently visible at:https://privacyinternational.org/node/4329*


# Title  #
Block Trackers on Firefox

# Summary #

Trackers are tools used by websites and apps to collect personal data about you, often with the goal of targeting you with ads. In this guide you'll learn how you can improve your online privacy by blocking trackers on Firefox.

# Body #
Online trackers are small bits of code embedded directly into a website's main code which collect data points about you and your browsing activity. This may include the pages you visit, how long you spend on them, where you scroll and the links you click on. On top of the online advertising industry, there are other actors that can potentially make use of trackers to track your online activity, including governments and/or law enforcement agencies.

There are extensions you can add to your browser that will limit the data collected by these trackers.

Warning: By blocking trackers you may cause some pages to display incorrectly or not at all. This guide also shows how you can modify the add-on's behaviour to allow some connections (see section on Disabling).

Note: There are many add-ons that block trackers. At PI we value open source and open-lists blockers as they are configurable and auditable. (see section on Selecting on why these characteristics matter)

Privacy Badger is an example of an open-source browser extension to block ads and trackers. 

Note that Privacy Badger is a project of the Electronic Frontier Foundation and its [privacy policy can be found here][1].


### Install ###
Like any other add-on, install Privacy Badger by visiting the [Mozilla Firefox Add-ons page][2] and clicking **Add to Firefox** (Fig. 1) and then clicking on **Add** when prompted (Fig. 2).

[1]: https://www.eff.org/code/privacy/policy
[2]: https://addons.mozilla.org/en-US/firefox/addon/privacy-badger17/

![Fig. 1: Download Privacy Badger](../../images/Firefox/badger-add.png?raw=true)

![Fig. 2: Add Privacy Badger to Firefox](../../images/Firefox/badger-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../../images/Firefox/badger-notify.png?raw=true)

Upon successful installation, a notification page opens on your browser and the Privacy Badger icon is added to the extension menu on your toolbar (Fig. 3). To pin the icon on the toolbar, click the extension menu, and then click the pin next to the Privacy Badger icon. 

Privacy Badger keeps an up-to-date list of known trackers that it finds through automated tests (not conducted from your computer but by dedicated servers), and regularly pushes the updated list to your browser. This means that as soon as new ad servers are detected (e.g. a new tracking company launches its product or an existing company deploys a new domain) they are blocked for Privacy Badger users. 

To learn more about how Privacy Badger works, click the icon and then click **Learn how Privacy Badger protects your privacy** (Fig. 4), or visit its [official documentation][3].

![Fig. 4: Learn more about Privacy Badger](../../images/Firefox/badger-learn.png?raw=true)

### Disabling
Blocking trackers and ads depends on knowing the lists of servers that serve ads and trackers. In some cases, a webpage might malfunction or refuse to load if a blocker is enabled. You can change the blocker's behaviour to allow select connections and exceptions. 

When using Privacy Badger, to allow a site to run trackers, you click on the toolbar icon and you can 'Disable for this site'. You can also make this change in Privacy Badger's settings under 'Disabled sites'. 

You can also alter the behaviours for specific trackers and cookies.

### Selecting Extensions/Add-ons

At PI we believe blockers should be open source and use open lists, as they can be audited. 

By using an independent, open-source and unencumbered/free blocker, you are more likely to avoid products with conflicts of interest, spyware or blockers with “acceptable ads” programs. 

With open source and open lists you can see what the blocker is doing, what will and won't be blocked. Open lists are often community-driven and updated frequently. 


[1]: https://www.eff.org/code/privacy/policy

[2]: https://addons.mozilla.org/en-US/firefox/addon/privacy-badger17/

[3]: https://privacybadger.org/
