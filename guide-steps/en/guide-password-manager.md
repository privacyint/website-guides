# Title
A guide for using a password manager

# Summary
A password manager is like having a vault for your online secrets, so that you have a safer online presence. In this guide, you will learn how to pick the right one, and easily fit it into your digital routine.

# Body

In the current digital landscape, passwords are the predominant method for user authentication across several platforms. From a privacy perspective, passwords present a distinctive advantage — unlike certain alternative authentication methods, they are not susceptible to physical coercion. Unlike biometric data or security hardware tokens, which can be physically compelled, passwords remain a confidential and non-coercible form of authentication. As such, they provide an additional layer of privacy protection.

Given the widespread adoption of passwords, managing multiple, unique passwords for each online account becomes more difficult. Having unique passwords for each account is a crucial step toward safeguarding your privacy, particularly in the face of potential data leaks. When reusing passwords, if one of your accounts suffers a data breach, this puts all your other accounts at risk. However, creating strong, unique passwords for each account is challenging and hard to remember for most individuals. We tend to lean towards familiar patterns or use easily memorable combinations, which, unfortunately, are also easier to crack. 

A password manager is a tool to solve these problems: it is designed to manage and store unique passwords for each online account. It functions as a secure repository, allowing users to generate and store complex credentials. By ensuring the strength, randomness, and uniqueness of each password, it minimizes the impact of potential data breaches, social engineering attacks, and brute-force hacking. In this guide, we highlight the key aspects you should look for in a password manager to ensure that your vault is private and secure.

- **Vault encryption**: Given that a file containing your passwords must exist somewhere, assess where the password manager stores this file whether — locally on your device or in the cloud. This can vault can either be stored in plaintext (meaning anyone can read its content) or encrypted (meaning only someone with the master password — you — can read its contents). Whether storing the vault locally or in the cloud, you should choose a password manager that stores its vault encrypted, as it provides an additional security layer in case the file is compromised. Look for robust encryption methods, such as AES-256, which ensures with a great degree of confidence that, even if unauthorized access occurs, the stored information remains unintelligible. Strong encryption is crucial, particularly for users with higher privacy concerns, such as activists or individuals living under oppressive regimes.

- **Vault location**: Opting for a local, encrypted vault provides an additional layer of privacy, as your sensitive data remains within your control. It ensures that, as long as you keep your devices safe, your vault is safe. On the other hand, if your device is unexpectedly compromised, you will lose access to your passwords, and possibly have them compromised. When working with a local vault, it is up to you to backup and keep the vault synced if you have multiple devices. In contrast, a cloud-based vault gives you strong availability guarantees and provide syncing effortlessly, so that you always have access to your vault even if you lose access to your device. However, using a cloud-based password manager introduces concerns about third-party access and the possibility of data breaches. It is crucial to scrutinize the security chain thoroughly, ensuring, for instance, that the cloud-based solution doesn't store sensitive information like master passwords in logs, as a breach in such logs could pose significant risks to your security. This information can typically be found summarized in security audits. Always exercise caution and diligence when considering a cloud-based password manager. 

- **Audited security practices**: Choose a password manager that undergoes regular security audits and is transparent about its practices. This provides a layer of assurance, as independent security assessments or audits offer external validation of the password manager's commitment to maintaining a high standard of security and privacy. Regular audits help ensure that the password manager is adhering to best practices and that potential vulnerabilities are promptly identified and addressed. Security audits provide an extra guarantee that the password manager prioritizes the security of your sensitive information.

- **Zero-Knowledge architecture**: Prioritize password managers that employ a zero-knowledge or zero-access architecture. This means that even the service provider cannot access your stored data or master password. This ensures an extra layer of security, especially relevant for individuals who may face targeted surveillance or persecution. If a provider of such a service is hacked or faces external pressures to disclose your data, the stored information remains unintelligible to whoever gains access, ensuring your passwords remain secure.

The following are examples of mainstream password managers:

- [Keepass](3) is an open-source, ad-, tracker-, and cloud-free password manager. It stores your passwords in a local, encrypted vault, and allows to you generate . It has been [audited by the EU-Free and Open Source Software Auditing Community](2), and has a proven track record of being safe and protecting your security. There are several clients you can use to interact with a Keepass vault. [KepassXC](https://keepassxc.org/) is a cross-platform client for desktop and mobile, that enables you to interact with your vault. It provides a browser extension to automatically fill login forms, save credentials when you creaate an online account, and provide you with random, unique, secure suggestions for passwords. On mobile devices, it integrates with your keyboard to provide credentials are an option, just like auto-complete.

![Keepass awards as displayed in their website](../../images/Password-Manager/keepass-awards.png?raw=true)

![KeepassXC integration on Android.](../../images/Password-Manager/keepass-android.jpg?raw=true)


- Apple's iCloud Keychain allows you to securely sync your passwords between your Apple devices without exposing that information to Apple. It provides a password manager with strong privacy and security guarantees. The password manager can automatically generate cryptographically strong password to use in Safari. In mobile devices, you can also use this functionality in apps. To learn how to setup iCloud Keychain on your device, see [this guide](5).

- Most common web browsers (Firefox, Chrome, Edge) provide you with a simple, cloud-based password manager to store your credentials so you can share them between multiple devices (i.e. cloud-based). Generally, these password managers do not provide you with suggestions for passwords, which is left up to you. As such, we only recommend their usage as a last resort (e.g. instead of writing password on post-it notes).


[1]: https://bitwarden.com/resources/zero-knowledge-encryption-white-paper/
[2]: https://joinup.ec.europa.eu/sites/default/files/inline-files/DLV%20WP6%20-02-%20Summary%20of%20the%20evaluation%20of%20results%20_KeePass_published.pdf
[3]: https://keepass.info
[4]: https://keepassxc.org/
[5]: https://support.apple.com/en-us/HT204085

Adopting a password manager serves as a crucial step in fortifying your online security and privacy, since passwords should be the preferred private authentication method When choosing a password manager, prioritize key features highlighted here, such as vault encryption, and adherence to best security practices. Choose a tool that aligns with your privacy preferences and security needs to safeguard your sensitive information in a secure way.