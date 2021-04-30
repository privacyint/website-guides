# Title  #
Install an ad-blocker on Microsoft Edge - uBlock Origin

# Summary #
uBlock Origin is a general purpose blocker for web browsers that blocks ads, trackers, and malware sites by default. In this guide, you'll learn how to install uBlock Origin on Microsoft Edge.

# Body #
uBlock Origin (not to be confused with uBlock which is a different project) is an independent and open-source ad blocker relying on a curated list of servers. It prevents your browser from connecting to these servers to serve you ads. 

> Note: There are many ad blockers on the market and you can test alternatives. By using an independent, open-source and free ad blocker, you are more likely to avoid products with conflicts of interest, spywares or blockers with "acceptable ads" programs. In theory, any ad blockers with open blacklisting and whitelisting that the user can edit should be able to offer similar results 

> **Warning**: Using an ad-blocker may cause some pages to display incorrectly or not at all. To prevent this behaviour, we show how to disable the extension in such cases.

### Installation ###
Like any other add-on, install uBlock Origin by visiting the [Microsoft Edge Add-ons Store][1] and clicking on **Get** (Fig. 1) and then clicking on **Add extension** when prompted (Fig. 2).

![Fig. 1: Download uBlock Origin](../../images/Edge/ublock-add.png?raw=true)

![Fig. 2: Add uBlock Origin to Edge](../../images/Edge/ublock-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../../images/Edge/ublock-notify.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the uBlock Origin icon is added to the extension menu on your toolbar (Fig. 3). To pin the icon on the toolbar, click the extension menu, and then click the pin next to the uBlock Origin icon. 

When you visit a website, uBlock Origin automatically blocks malicious trackers and ads, which you can check by clicking the icon (Fig. 4).

![Fig. 4: uBlock Origin pop-up interface](../../images/Edge/ublock-test.png?raw=true)

### Whitelisting
In some case, a webpage might malfunction or refuse to load if uBlock Origin is enabled. In this case, you can disable uBlock Origin for a given website by clicking on the icon and then click on the large power button (Fig. 4). Simply reload the page either by clicking the reload icon on uBlock Origin (Fig. 5) or by refreshing the page in your browser.

Note that using Ctrl+click will disable temporarily uBlock Origin instead of disabling it on this site entirely and indefinitely.

![Fig. 5: uBlock Origin whitelist a domain](../../images/Edge/ublock-whitelist.png?raw=true)

uBlock Origin is a powerful, highly configurable tool to block any network request on your browser. If you are interested in more advanced usage, visit the [official documentation page][2].

[1]: https://microsoftedge.microsoft.com/addons/detail/ublock-origin/odfafepnkmbhccpbejgmiehpchacaeak

[2]: https://github.com/gorhill/uBlock/wiki
