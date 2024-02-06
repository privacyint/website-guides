# Title #
A guide to keeping your mobile phone's location history private

# Summary #
Carrying your phone with an always-on GPS chip means mobile devices can track your every move and build a profile based on your location history. In this guide, we'll take you through steps you can take to keep your location history private. 

# Body #
In your day-to-day life, your smartphone silently captures and stores a digital footprint of your whereabouts by keeping a *location history*: this history is then used to enhance your mobile experience, such as by aiding in navigation and customizing app experiences according to your location habits. 

Yet, it's essential to recognize the potential risks tied to this seemingly innocuous practice. Understanding how your location data is handled becomes vital, as it can impact your privacy in ways you might not have considered. Particularly, you should be aware of the following concerns:

- **Cloud vulnerabilities**: Storing location history in the cloud poses a potential risk if the cloud service is compromised (e.g. a data breach). Unauthorized access to cloud-stored location data can reveal your detailed movement patterns, potentially leading to stalking, harassment, or other malicious activities.

- **Local device compromise**: Even if your location history is kept on your device only, it still poses a privacy risk. If your mobile device is compromised, whether through theft, hacking, or taken by force (e.g. at border control), an attacker can retrieve your stored location history. This provides them with a detailed record of your past movements and most frequently visited places, which may then be used against you.

- **Third-party app misuse**: Some third-party apps may request access to location data for seemingly innocuous purposes but can misuse this information for targeted advertising, profiling, or selling data to third parties without the user's explicit consent. In these cases, typically, the operating system provides a way for you to limit app access to your location data.

- **Government surveillance**: In regions where government surveillance is a concern, location history can be used to track individuals' movements, potentially infringing on civil liberties and posing risks to personal safety.

- **Data aggregation and inference**: Aggregating location data from various sources can enable the creation of a detailed user profile, allowing companies or adversaries to infer sensitive information about an individual's habits, preferences, and lifestyle, leading to potential privacy violations.

As location tracking becomes increasingly integrated into our digital lives, understanding and managing the associated privacy risks are crucial for protecting your privacy. The rest of this guide explains how to disable this feature on both Android and iOS.

### Android
If you have a Google account associated with your Android device, chances are your location history is being stored. Recently, Google decided it will soon [stop storing your location stored on the cloud][1]: however, it is still stored on your device, posing a potential privacy risk.

To disable location history, go to your Google account settings. You can do so by visting [this link][2], opening the settings app on your device, or using the Google app. In the account settings, find the **Data & privacy** tab. 

![Google account data & privacy settings.](../../images/Google/google-privacy-settings.jpg?raw=true)

Scroll down until you see the **History settings** section. Click on **Location History**, and then disable it. This should prevent Google from collection your location history and storing it on their servers and your device.

![Google account location history settings.](../../images/Google/google-location-history.jpg?raw=true)


### iOS
Unlike Google, Apple keeps most of your location history on your device: the bits of information stored in the cloud are either [end-to-end encrypted][3], meaning only you can decipher them, or anonymized. As such, the risk of having your location history compromised by a data breach, or by a request from law enforcement to Apple for this data, is greatly reduced. However, as we explained earlier, having your location history stored on your device(s) still poses a privacy risk.

To disable location history, go to **Settings > Privacy > Location services** and then scroll down until you find the **System services** option.

![Apple privacy setting for location services.](../../images/ios/apple-location.jpg?raw=true)

In the **System services** screen, you can select which system applications have access to your location. To prevent location history from being stored on your iCloud-connected devices, select the **Significant locations** option.

![Apple system services location settings.](../../images/ios/apple-location-history.jpg?raw=true)

In this screen, you can see an overview of your location history and your most frequently-visited places. Start by clearing the history by clicking the **Clear History** button on the bottom of the page. Finally, to disable the storage of location history, toggle the **Significant Locations** option at the top of the page.

![Disable location history on iOS](../../images/ios/apple-location-significant.jpg?raw=true)

Note that if you use any Google service, tied to your Google account, on your iOS device (e.g. Google Maps), you should follow the same steps in the previous section, to prevent location history from being stored in your Google account.

[1]: https://blog.google/products/maps/updates-to-location-history-and-new-controls-coming-soon-to-maps/
[2]: https://www.google.com/account/about
[3]: https://www.apple.com/legal/privacy/data/en/location-services/