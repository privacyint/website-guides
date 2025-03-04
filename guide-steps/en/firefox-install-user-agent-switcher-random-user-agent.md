**Currently visible at: https://privacyinternational.org/node/4324**

# Title #
Install a user agent switcher on Firefox

# Summary #
In this guide, you'll learn how to periodically change your browser's user agent and make it harder for trackers to fingerprint you.

# Body #
When you access a website, your browser sends a string called the *User Agent* containing your browser's name, operating system, and other technical metadata of your device. Unfortunately, this metadata is often abused by trackers to build a *fingerprint* of your system and uniquely identify you throughout the web. To limit the efficiency of fingerprinting you can install a random agent switcher which periodically changes your browser's user agent, making it harder to uniquely identify you.

Random User Agent is an [open source](https://github.com/tarampampam/random-user-agent) add-on that allows you to do this.

> **Note**: There are likely other add-ons or apps available and you can test alternatives. At PI we believe add-ons/apps should be open source as they can be audited. By using an independent, open-source and unencumbered/free add-on/app, you are more likely to avoid products with conflicts of interest, spyware, data-leakage, or blockers with “acceptable ads” programs. Here we show the set-up and settings of one such add-on/app that we’ve used at PI; others are likely similar with varying levels of configurability.

> **Warning**: Using an agent switcher may cause some pages to display incorrectly or not at all. To prevent this behaviour, we show how to disable the extension in such cases.

### Installation ###
Like any other add-on, install Random User Agent by visiting the [Mozilla Firefox Add-ons page][1] and clicking **Add to Firefox** (Fig. 1) and then clicking on **Add** when prompted (Fig. 2).

![Fig. 1: Download Random User Agent](../../images/Firefox/agent-add.png?raw=true)

![Fig. 2: Add Random User Agent to Firefox](../../images/Firefox/agent-prompt.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and the Random User Agent icon is added to your toolbar (Fig. 3).

![Fig. 3: Notification of successful installation](../../images/Firefox/agent-notify.png?raw=true)

To check your currently assigned user agent, click the icon (Fig. 4). If you stumble on a page which breaks when you have Random User Agent enabled, you can either disable it for that domain, clicking on **Enabled on this domain**, or pause the switcher temporarily, clicking on **Pause Switcher**.

![Fig. 4: Random User Agent pop-up interface](../../images/Firefox/agent-test.png?raw=true)

Random User Agent is configured by default to change the user agent every 10 minutes, although you can configure this in the settings (Fig. 5).

![Fig. 5: Random User Agent settings page](../../images/Firefox/agent-settings.png?raw=true)

[1]: https://addons.mozilla.org/en-US/firefox/addon/random_user_agent/
