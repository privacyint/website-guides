*Currently visible at: https://privacyinternational.org/node/3392*

# Title  #
Block Ads on Chrome (and derivatives)

# Summary #
Ad Blockers prevent your browser from connecting to servers that serve you ads, which can minimise the amount of data you share with third parties. In this guide, you'll learn how to install an Ad Blocker on Chrome and its derivatives (Opera, Chromium, Brave...)

# Body #

Ad Blockers aim to prevent your browser from connecting to Ad servers and loading ads on webpages you are visiting. They can also block some parts of webpages that likely display ads. Blocking ads and connections to ad servers can help minimise the amount of data that the Adtech industry collects about you for targeted advertising. 
    
> Warning: Using an ad-blocker may cause some pages to display incorrectly or not at all. This guide also shows how you can modify the Ad Blocker's behaviour to allow some connections (see section on Disabling).
    
> Note: There are many ad blockers available. At PI we value open source and open-lists ad blockers as they are configurable and auditable. (see section on Selection on why these characteristics matter)

uBlock Origin (not to be confused with uBlock which is a different project) is one example of an independent, [open-source][2] and configurable Ad Blocker relying on open lists of ad servers. 

### Install ###
Like any other add-on, install uBlock Origin by visiting the [Chrome Web Store][1] and clicking on **Add to Chrome** (Fig. 1) and then clicking on **Add extension** when prompted (Fig. 2).

![Fig. 1: Download uBlock Origin](../../images/Chrome/ublock-add.png?raw=true)

![Fig. 2: Add uBlock Origin to Chrome](../../images/Chrome/ublock-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../../images/Chrome/ublock-notify.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the uBlock Origin icon is added to the extension menu on your toolbar (Fig. 3). To pin the icon on the toolbar, click the extension menu, and then click the pin next to the uBlock Origin icon. 

When you visit a website, uBlock Origin uses open-lists to block trackers and ads, which you can check by clicking the icon (Fig. 4).

![Fig. 4: uBlock Origin pop-up interface](../../images/Chrome/ublock-test.png?raw=true)

### Disabling
Effective ad blocking depends on knowing the lists of servers that serve ads. In some cases, a webpage might malfunction or refuse to load if an Ad blocker is enabled. You can change the Ad Blocker's behaviour to allow select connections and exceptions. 

You can disable uBlock Origin for a given website by clicking on the icon and then click on the large power button (Fig. 4). Simply reload the page either by clicking the reload icon on uBlock Origin (Fig. 5) or by refreshing the page in your browser.
    
![Fig. 5: uBlock Origin disabling blocking for a domain](../../images/Chrome/ublock-whitelist.png?raw=true)

If you are interested in more advanced use, visit the [official documentation page][2].

### Selecting Ad Blockers

At PI we believe Ad Blockers should be open source and use open lists. 

By using an independent, open-source and unencumbered/free ad blocker, you are more likely to avoid products with conflicts of interest, spyware or blockers with “acceptable ads” programs. 

With open source and open lists you can inspect what the adblocker is doing, what will and won't be blocked. Open lists are often community-driven and updated frequently. 

[1]: https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm

[2]: https://github.com/gorhill/uBlock/wiki
