# Title #
Install a cookie manager on Firefox - Cookie AutoDelete

# Summary #

Browser cookies allow websites to preserve session data such as your login credentials or items in your shopping basket
so that you don't lose information when you close the page. Unfortunately, they are often abused to track your online
activity across the web. In this guide you'll learn how to install Cookie AutoDelete, a web-browser add-on that
automatically deletes unused cookies.

# Body #

### Installation ###

Like any other add-on, install Cookie AutoDelete by visiting the [Mozilla Firefox Add-ons
page](https://addons.mozilla.org/en-US/firefox/addon/cookie-autodelete/) and clicking **Add to Firefox** (Fig. 1) and
then clicking on **Add** when prompted (Fig. 2).

![Fig. 1: Download Cookie AutoDelete](../images/Firefox/cad-add.png?raw=true)

![Fig. 2: Add Cookie AutoDelete to Firefox](../images/Firefox/cad-prompt.png?raw=true)

![Fig. 3: Notification of successful installation](../images/Firefox/cad-notify.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the Cookie AutoDelete icon is added to
your toolbar (Fig. 3). When you visit a website, the Cookie AutoDelete icon shows the number of stored cookies for that
website. By clicking the icon (Fig. 4), you are able to clean cookies, and also whitelist (permanently) or greylist
(until a browser restart) websites you trust to store cookies.

![Fig. 4: Cookie AutoDelete pop-up interface](../images/Firefox/cad-test.png?raw=true)

The extension disables automatic cleanup by default. To enable it, click the icon (Fig. 4) and then click on
**Auto-clean disabled**. That way, you don't have to remember to manually clean your cookies: when you close a browser
tab, any cookies no longer in use are automatically deleted.

### Avoid tracking from whitelisted cookies ###

![Fig. 5: Disable support for Firefox Containers](../images/Firefox/cad-containers.png?raw=true)

If you want to disable Cookie AutoDelete for some website (e.g. your email client), you can whitelist it by clicking the
icon and then clicking on **Whitelist** (Fig. 4). However, note that whitelisted cookies may still communicate between themselves
and temporary cookies, thus tracking your activity. The two options below help you avoid this behaviour.

#### Use Firefox Multi-Containers ####

To ensure cookies from whitelisted domains remain isolated, you can create one container for each whitelisted domain. To
learn more about Firefox Multi-Account Containers read [our guide on how to set it up](firefox-containers.md). For this
to work, it's important to keep the setting **Enable Support for Firefox's Container Tabs** disabled (Fig. 5).

#### Enable First Party Isolation ####

You can also enable First Party Isolation so that cookies from different domains are isolated. This is the most
effective way to ensure temporary cookies do not cross-reference your activity before they are deleted. Note, however,
that this may introduce some performance penalty. To learn how to enable First Party Isolation in Firefox, read our guide
on [Firefox privacy settings](firefox-settings.md).
