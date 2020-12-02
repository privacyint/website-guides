# Title #
Adjusting Chrome (and derivatives) settings to enhance your online privacy

# Summary #
In this guide you'll learn how to configure your Chrome browser settings to harden your online privacy.

# Body #

> **Warning:** Google Chrome employs a mechanism to automatically link your browser to your Google account when you sign
> in on any Google service (e.g. Gmail). This inevitably links your browser activity to your Google account. Consider
> using a Chrome-based alternative (e.g. Brave, Opera) to avoid this, or alternatively disable this in the settings (we
> illustrate how to so in this guide).

### Changing settings in Chrome menu ###
To access the settings, click on the three-dot menu on the upper right and then press **Settings** (Fig. 1), or type
<chrome://settings/> in the URL bar and press Enter.

![Fig. 1: Chrome settings menu](../images/Chrome/settings-menu.png?raw=true)

#### You and Google ####
Chrome includes several features meant to improve your browsing experience that require you to share data with
third-parties. You can disable this options by going to the Settings page, and clicking on **You and Google** > **Sync
and Google Services**. Disable **Autocomplete searches and URLs**, **Make searches and browsing better**, and **Allow
Chromium sign-in** to prevent this data from being sent to Google's servers (Fig. 2).

![Fig. 2: Sync settings](../images/Chrome/settings-sync.png?raw=true)

#### Privacy and security ####
On the Settings page, click on **Privacy and security**. In this page you can change some settings to protect yourself
from online trackers.

##### Cookies and other site data #####
When browsing the web, your browser may warn websites that you do not want to be tracked. Beware that not all websites
respect this! For safer protection, please see [our guide on installing an ad-blocker](chrome-ublock-origin.md). Still,
it's better to have this option turned on. Enable **Send a "Do Not Track" request with your browsing traffic**, and
disable **"Preload pages for faster browsing and searching"**.

##### Security #####
Enable **Standard protection** on the Safe Browsing settings [^1]. Then, click the arrow on the right to open the advanced
settings panel. Disable **Help improve security on the web for everyone** (Fig. 3).

[^1]: You may want to use enhanced protection but be aware that this requires additional data to be sent to Google.

![Fig. 3: Security settings](../images/Chrome/settings-security.png?raw=true)

##### Site settings #####
On the permissions section, enable **Ask before accessing** on **all** permissions, and disable **Background sync**.
Scroll to the bottom of the page and click on **Additional content settings**, and disable **Ads**.

![Fig. 4: Permission settings](../images/Chrome/settings-permissions.png?raw=true)
