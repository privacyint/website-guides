# Title #
Install a cookie manager on Chrome (and derivatives) - Cookie AutoDelete

# Summary #
Browser cookies can be useful but are often abused to track your online activity across the web. In this guide you'll learn how to install Cookie AutoDelete, a web-browser add-on that automatically deletes unused cookies.

# Body #
Browser cookies allow websites to preserve session data such as your login credentials or items in your shopping basket so that you don't lose information when you close the page. Unfortunately, they are often abused to track your online activity across the web. Using a dedicated addon, you can clean your cookies regularily to ensure that no unwanted cookie is kept in your browser, limiting the efficienty of online trackers.

This guide explain how to install Cookie AutoDelete, a web-browser add-on that automatically deletes unused cookies.

> **Warning**: Cookies are widely used on the web and this extension might break some website features. Be sure to understand what it does and how to disable it before installing it!

### Installation ###
Like any other add-on, install Cookie AutoDelete by visiting the [Chrome Web Store][1] and clicking on **Add to Chrome** (Fig. 1) and then clicking on **Add extension** when prompted (Fig. 2).

![Fig. 1: Download Cookie AutoDelete](../../images/Chrome/cad-add.png?raw=true)

![Fig. 2: Add Cookie AutoDelete to Chrome](../../images/Chrome/cad-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../../images/Chrome/cad-notify.png?raw=true)

Upon successful installation you'll see the Cookie AutoDelete Welcome page (Fig. 3), and the extension icon is added to your toolbar. When you visit a website, the Cookie AutoDelete icon shows the number of stored cookies for that website. By clicking the icon (Fig. 4), you are able to clean cookies, and also whitelist (permanently) or greylist (until a browser restart) websites you trust to store cookies.

![Fig. 4: Cookie AutoDelete pop-up interface](../../images/Chrome/cad-test.png?raw=true)

The extension disables automatic cleanup by default. To enable it, click the icon (Fig. 4) and then click on **Auto-clean disabled**. That way, you don't have to remember to manually clean your cookies: when you close a browser tab, any cookies no longer in use are automatically deleted. This is a double edged swords: this means that all tracking cookies will be deleted but also means you will be logged out of any session you currently had open. Enabling this option is equivalent to "starting anew" every time you open your browser (although you can keep your tabs open, you won't be logged in anywhere apart from the website you whitelisted).

### Avoid tracking from whitelisted cookies ###

If you want to disable Cookie AutoDelete for some website (e.g. your email client), you can whitelist it by clicking the icon and then clicking on **Whitelist** (Fig. 4). However, note that whitelisted cookies may still communicate between themselves and temporary cookies, thus tracking your activity. The two options below help you avoid this behaviour.

Adding a site to the whitelist is particularily useful if you want to stay connected on a particular site (like your email account) even after your restart your browser.

[1]: https://chrome.google.com/webstore/detail/cookie-autodelete/fhcgjolkccmbidfldomjliifgaodjagh
