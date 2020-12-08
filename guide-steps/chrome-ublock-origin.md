# Title  #
Install an ad-blocker on Chrome (and derivatives) - uBlock Origin

# Summary #
uBlock Origin is a general purpose blocker for web browsers that blocks ads, trackers, and malware sites by default. In this guide, you'll learn how to install uBlock Origin on Chrome and its derivatives (Opera, Chromium, Brave...)

# Body #

uBlock Origin (do not mistake with uBlock which a completely different project) is an independant and open-source ad-blocker relying on a currated list of servers. It prevents your browser from connecting to these servers to serve you ads. We recommand it over AdBlock Plus which authorise certain ads to be displayed according to its ["Acceptable Ads program"](https://acceptableads.com/).

> Notes: There are other ad-blockers on the market and you are free to test other alternatives. But we recommand you use an independant, open-source and free ad-blocker to avoid products with conflict of interest, spywares or blockers with "acceptable ads" program. Ad-blockers with open blacklisting and whitelisting that the user can edit should be able to get you through

> **Warning**: Using an ad-blocker may cause some pages to display incorrectly or not at all. To prevent this behaviour, we show how to disable the extension in such cases.

### Installation ###
Like any other add-on, install uBlock Origin by visiting the [Chrome Web Store][1] and clicking on **Add to Chrome** (Fig. 1) and then clicking on **Add extension** when prompted (Fig. 2).

![Fig. 1: Download uBlock Origin](../images/Chrome/ublock-add.png?raw=true)

![Fig. 2: Add uBlock Origin to Chrome](../images/Chrome/ublock-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../images/Chrome/ublock-notify.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the uBlock Origin icon is added to the extension menu on your toolbar (Fig. 3). To pin the icon on the toolbar, click the extension menu, and then click the pin next to the uBlock Origin icon. 

When you visit a website, uBlock Origin automatically blocks malicious trackers and ads, which you can check by clicking the icon (Fig. 4).

![Fig. 4: uBlock Origin pop-up interface](../images/Chrome/ublock-test.png?raw=true)

In some case, a webpage might malfunction or refuse to load if uBlock Origin is enabled. In this case, you can disable uBlock Origin for a given website by clicking on the icon and then click on the large power button (Fig. 4). Simply reload the page either by clicking the reload icon on uBlock Origin (Fig. 5) or by refreshing the page in your browser.

Note that using Ctrl+click will disable temporarily and uBlock Origin instead of disabling it on this site entirely .

![Fig. 5: uBlock Origin whitelist a domain](../images/Chrome/ublock-whitelist.png?raw=true)

uBlock Origin is a powerful, highly configurable tool to block any network request on your browser. If you are interested in more advanced usage, visit the [official documentation page][2].

[1]: https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm

[2]: https://github.com/gorhill/uBlock/wiki
