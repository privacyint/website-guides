# Title #
Install a user agent switcher on Chrome (and derivatives) - Random User Agent

# Summary #
When you access a website, your browser sends a string called the *User Agent*
containing your browser's name, operating system, and other technical metadata
of your device. Unfortunately, this metadata is often abused by trackers to
build a *fingerprint* of your system and identify you throughout the web.

In this guide, you'll learn how to install Random User Agent on Chrome (and
derivatives) to periodically change your browser's user agent and make it harder
for trackers to fingerprinting you.

# Body #
> **Warning**: Using an agent switcher may cause some pages to display
> incorrectly or not at all. To prevent this behaviour, we show how to disable
> the extension in such cases.

### Installation ###
Like any other add-on, install Random User Agent by visiting the [Chrome Web
Store][1] and clicking on **Add to Chrome** (Fig. 1) and then clicking on **Add
extension** when prompted (Fig. 2).

![Fig. 1: Download Random User Agent](../images/Chrome/agent-add.png?raw=true)

![Fig. 2: Add Random User Agent to
Firefox](../images/Chrome/agent-prompt.png?raw=true)

Upon successful installation a notification appears on the top-right corner, and
the Random User Agent icon is added to your toolbar (Fig. 3).

![Fig. 3: Notification of successful
installation](../images/Chrome/agent-notify.png?raw=true)

To check you currently assigned user-agent, click the icon (Fig. 4). If you
stumble on a page which breaks when you have Random User Agent enabled, you can
either disable it for that domain, clicking on **Enabled on this domain**, or
pause the switcher temporarily, clicking on **Pause Switcher**.

![Fig. 4: Random User Agent pop-up
interface](../images/Chrome/agent-test.png?raw=true)

Random User Agent is configured by default to change the user agent every 10
minutes, although you can configure this in the settings (Fig. 5).

![Fig. 5: Random User Agent settings
page](../images/Chrome/agent-settings.png?raw=true)

[1]: https://chrome.google.com/webstore/detail/random-user-agent/einpaelgookohagofgnnkcfjbkkgepnp
