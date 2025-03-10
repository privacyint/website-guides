**Currently visible at: https://privacyinternational.org/node/5536**

# Title
A guide for using privacy-focused alternative frontends to mainstream websites

# Summary
Popular Internet platforms, such as YouTube or X (formerly Twitter), are not particularly famous for respecting your privacy. To help preserve your privacy while still being able to access the content of these platforms, you can make of use alternative front-ends. In this guide you will learn how to choose and setup alternative front-ends on your desktop and mobile devices.

# Body

Many mainstream Internet platforms, such as YouTube and X, often collect extensive user data, track online activities, and employ algorithms to create content recommendations based on individual preferences. For a privacy-conscious user, this is nothing short of a nightmare. Making use of alternative front-ends allows you to access the content you want, while minimising the data collected about you. Essentially, this corresponds to using a different website to access the same content. By using alternative interfaces, you can avoid some of the data tracking mechanisms employed by major platforms, thus preserving a higher level of anonymity and control over your online presence.

Alternative front-ends often prioritize open-source and decentralized models, offering users more transparency and control over how their data is handled (e.g. not storing it on the cloud). Decentralized platforms often distribute data across multiple servers, reducing the risk of centralized data breaches. The absence of targeted advertisements that are prevalent on mainstream platforms, and [which usually rely heavily on user personal data](https://privacyinternational.org/learn/micro-targeting), is a common feature in alternative front-ends, as they tend to adopt different monetization models that don't rely on extensive user profiling and data collection (e.g. donations). Opting for alternative front-ends minimizes your exposure to certain privacy risks associated with popular, data-driven platforms.

### Alternative front-ends

There are many available alternative front-ends for popular online platforms. When looking for an alternative front-end, you may want to consider the following aspects:

1. **Data handling practices**: Evaluate how the alternative front-end manages user data. Opt for platforms that minimize data collection — preferably keeping it local-only — and have transparent privacy policies. Look for alternatives that prioritize user privacy by avoiding excessive tracking and data retention practices.
2. **Open Source and transparency**: Choose alternative front-ends that are open source and transparent about their codebase. Open-source projects allow users to inspect the code, fostering trust and ensuring that the platform operates with integrity. Since the code is available, anyone is free to inspect it for possible attacks (e.g. see [here](https://github.com/iv-org/invidious/issues/1456) for an example where a user detected a privacy violation in a YouTube alternative instance, leading the project developer to remove it from the list of suggested instances.)
3. **Decentralization and user control**: Look for alternatives that follow decentralized models and provide users with greater control over their data. Platforms that distribute data across multiple instances or offer features allowing users to manage their information effectively contribute to a more privacy-centric experience. Decentralized systems also reduce the risk of single-point failures and large-scale data breaches.

Nitter and Invidious, alternative front-ends to X and YouTube respectively, are two examples, among many, that satisfy all the above requirements. For a more extensive list of alternatives to popular platforms, refer to [this page](https://github.com/digitalblossom/alternative-frontends).

[Nitter][https://nitter.space/] is a free and open source alternative X front-end focused on privacy and performance that allowed you to search and read tweets without requiring an account and without collecting any data on your activity. Nitter.com has been discontinued but there are many alternative similar instances you can find on [this page](https://status.d420.de/). Nitter instances are also ~15 times lighter than X's, which is particularly relevant if you're on a capped mobile data plan. 

If you want to open a X link in Nitter, simply replace the **X.com** in the URL with the link to a Nitter instance (e.g. nitter.space). For instance, our X page, X.com/privacyint, can be found on Nitter at the URL [nitter.space/privacyint][https://nitter.net/privacyint] 

![Privacy International page on Nitter.](../../images/Alternative-Frontends/nitter-pi.png?raw=true)

[Invidious](https://invidious.io/) is a free and open source alternative to YouTube. It  minimizes the extent of data exchanged with Google, providing a YouTube-like experience with reduced tracking. By avoiding direct interaction with the YouTube website, you can access and watch videos with a certain degree of anonymity, as your activity is not as closely tied to your Google account, nor linked to other online trackers: Invidious itself does not collect any data on your activity, unlike YouTube.

Invidious offers features such as the ability to watch videos, view comments, and subscribe to channels. Additionally, Invidious provides options for users to customize their experience, and it is often used by individuals who are concerned about privacy and data collection on mainstream platforms.

Similarly to Nitter, Invidious is also decentralized. You can check [here](https://docs.invidious.io/instances/) for a list of public instances. 

If you want to open a YouTube link in Invidious, simply replace the **youtube.com** in the URL with the link to a Invidious instance (e.g. yewtu.be). For instance, our YouTube channel, youtube.com/@privacyint, can be found on Invidious at [yewtu.be/@privacyint](https://yewtu.be/channel/UCwyKZWhsD2YFg8huOaO3IOg).

![Privacy International channel on Invidious.](../../images/Alternative-Frontends/invidious-pi.png?raw=true)


### Use alternative front-ends in your web browser
To simplify the process of using alternative front-ends in your web browser, you can use a browser extension that automatically redirects URLs to the chosen front-end, eliminating the need for manual redirection. 

One example of such an extension is [Redirector](https://github.com/einaregilsson/Redirector), a general purpose URL rewriter that is available for most common web browsers (Firefox, Vivaldi, Chrome, Opera, Edge). It allows users to redirect any URLs based on regular expressions or wildcard patterns.

![Main page of the Redirector extension.](../../images/Alternative-Frontends/redirector-home.png?raw=true)

This extension is useful if you always want to redirect links to alternative front-ends without having to manually change the links. For example, if you always want to open X links in Nitter, you can set up the following redirect after installing the extension.

![Set up extension to redirect X to Nitter](../../images/Alternative-Frontends/redirect-rule.png?raw=true)

To learn how to redirect YouTube links to an Invidious instance with Redirector, you can read [this guide](https://docs.invidious.io/redirector/).

### Use alternative front-ends in your mobile device
In mobile devices, besides the web browser, you can also use apps that work with alternative front-ends instead of communicating with the online service directly. These typically store your data locally, without sharing it with third parties, and do not require accounts for you to use them. For instance, if you wish to use an alternative, privacy-respecting, front-end to X, you can install the [Fritter](https://fritter.cc/) app; if you want an alternative to the YouTube app, you can use [Clipious](https://github.com/lamarios/clipious) or [NewPipe](https://newpipe.net/). All are available for Android. In iOS, there are fewer options (e.g. [Yattee](https://apps.apple.com/us/app/yattee/id1595136629?platform=iphone), an app for Invidious); however, you can still use the web browser to access alternative front-ends, as you would on a desktop computer.

![NewPipe on Android showing our YouTube channel](../../images/Alternative-Frontends/newpipe-pi.jpg?raw=true)

Alternative front-ends may actually provide you with more features than the original service. As examples, the NewPipe app lets you play YouTube videos in the background, create and manage playlists without needing an account, and download videos; the Fritter app allows you to bookmark tweets, find users and tweets, follow and group accounts, all without requiring that you have an account of your own.

[1]: https://fritter.cc/
[2]: https://github.com/lamarios/clipious
[3]: https://newpipe.net/
[4]: https://github.com/iv-org/invidious/issues/1456
[5]: https://nitter.net/ 
[6]: https://github.com/zedeus/nitter/wiki/Instances
[7]: https://nitter.net/privacyint
[8]: https://apps.apple.com/us/app/yattee/id1595136629?platform=iphone
[9]: https://docs.invidious.io/instances/
[10]: https://yewtu.be/@privacyin
[11]: https://github.com/einaregilsson/Redirector
[12]: https://docs.invidious.io/redirector/
[13]: https://privacyinternational.org/learn/micro-targeting
[14]: https://github.com/digitalblossom/alternative-frontends
[15]: https://invidious.io/
