**Currently visible at: https://privacyinternational.org/node/4325**


# Title #
Install a cookie manager on Firefox

# Summary #
Browser cookies can be useful but are often abused to track your online activity across the web. In this guide you’ll learn how to install Cookie AutoDelete, a web-browser add-on that automatically deletes unused cookies.

# Body #
Browser cookies allow websites to preserve session data such as your login credentials or items in your shopping basket so that you don't lose information when you close the page. Unfortunately, they are often abused to track your online activity across the web. Using a dedicated add-on, you can clean your cookies regularly to ensure that no unwanted cookie is kept in your browser, limiting the efficiency of online trackers.

This guide explain how to install Cookie AutoDelete, an [open-source](https://github.com/Cookie-AutoDelete/Cookie-AutoDelete) web-browser add-on that helps you manage your cookies in automated ways.

> **Warning**: Cookies are widely used on the web and this extension might break some website features. Be sure to understand what it does and how to disable it before installing it!

> Note: There are likely other add-ons or apps available and you can test alternatives. At PI we believe add-ons/apps should be open source as they can be audited. By using an independent, open-source and unencumbered/free add-on/app, you are more likely to avoid products with conflicts of interest, spyware, data-leakage, or blockers with “acceptable ads” programs. Here we show the set-up and settings of one such add-on/app that we’ve used at PI; others are likely similar with varying levels of configurability.

### Installation ###

Like any other add-on, install Cookie AutoDelete by visiting the [Mozilla Firefox Add-ons page][1] and clicking **Add to Firefox** (Fig. 1) and then clicking on **Add** when prompted (Fig. 2).

![Fig. 1: Download Cookie AutoDelete](../../images/Firefox/cad-add.png?raw=true)

![Fig. 2: Add Cookie AutoDelete to Firefox](../../images/Firefox/cad-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../../images/Firefox/cad-notify.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the Cookie AutoDelete icon is added to your toolbar (Fig. 3). When you visit a website, the Cookie AutoDelete icon shows the number of stored cookies for that website. By clicking the icon (Fig. 4), you are able to clean cookies, and also "whitelist" (permanently) or greylist (until a browser restart) websites you trust to store cookies.

![Fig. 4: Cookie AutoDelete pop-up interface](../../images/Firefox/cad-test.png?raw=true)

The extension disables automatic clean-up by default. To enable it, click the icon (Fig. 4) and then click on **Auto-clean disabled**. That way, you don't have to remember to manually clean your cookies: when you close a browser tab, any cookies no longer in use are automatically deleted. This is a double edged sword: this means that all tracking cookies will be deleted but also means you will be logged out of any session you currently had open. Enabling this option is equivalent to "starting anew" every time you open your browser (although you can keep your tabs open, you won't be logged in anywhere apart from the website you "whitelisted").

### Avoid tracking from "whitelisted" cookies ###

If you want to disable Cookie AutoDelete for some website (e.g. your email client), you can "whitelist" it by clicking the icon and then clicking on **Whitelist** (Fig. 4). However, note that "whitelisted" cookies may still communicate between themselves and temporary cookies, thus tracking your activity. The options below help you avoid this behaviour.

Adding a site to the "whitelist" is particularly useful if you want to stay connected on a particular site (like your email account) even after your restart your browser.

#### Use Firefox Total Cookie Protection ####
To ensure cookies from different domains remain isolated, you should enable Total Cookie Protection. This prevents websites from tracking you with cookies across different domains (e.g. if you visit Facebook, they won't be able to read cookies from other websites you visit). It should be enabled by default after you install Firefox. To learn more about Firefox Total Cookie Protection read [our guide on Firefox privacy settings][3].

#### Use Firefox Multi-Containers ####

Total Cookie Protection only works for different domains. If you want to isolate cookies from the same domain (e.g. Google Shopping and Google News), you can create one container for each domain. To learn more about Firefox Multi-Account Containers read [our guide on how to set it up][2]. For this to work, it's important to keep the setting **Enable Support for Firefox's Container Tabs** enabled (Fig. 5).

![Fig. 5: Disable support for Firefox Containers](../../images/Firefox/cad-containers.png?raw=true)

#### Enable First Party Isolation ####

You can also enable First Party Isolation so that cookies from different domains are isolated. This is the most effective way to ensure temporary cookies do not cross-reference your activity before they are deleted. To learn how to enable or disable First Party Isolation in Firefox, read our guide on [Firefox privacy settings][3].

[1]: https://addons.mozilla.org/en-US/firefox/addon/cookie-autodelete/

[2]: http://privacyinternational.org/guide-step/4327/firefox-isolating-your-online-activity-multi-account-containers

[3]: http://privacyinternational.org/guide-step/4330/firefox-adjusting-settings-enhance-your-online-privacy

