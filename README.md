[![Bread](/images/top-logo.png)](https://itunes.apple.com/app/breadwallet/id885251393)

## The easy and secure bitcoin wallet

BRD is the best way to get started with bitcoin. Our simple, streamlined design is easy for beginners, yet powerful enough for experienced users.

### Completely decentralized

Unlike other iOS bitcoin wallets, **BRD** is a standalone bitcoin client. It connects directly to the bitcoin network using [SPV](https://en.bitcoin.it/wiki/Thin_Client_Security#Header-Only_Clients) mode, and doesn't rely on servers that can be hacked or disabled. Even if BRD the company disappears, the app will continue to function, allowing users to access their money at any time.

### Cutting-edge security

**BRD** utilizes AES hardware encryption, app sandboxing, and the latest iOS security features to protect users from malware, browser security holes, and even physical theft. Private keys are stored only in the secure enclave of the user's phone, inaccessible to anyone other than the user.

### Desgined with new users in mind

Simplicity and ease-of-use is **BRD**'s core design principle. A simple recovery phrase (which we call a paper key) is all that is needed to restore the user's wallet if they ever lose or replace their device. **BRD** is [deterministic](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki), which means the user's balance and transaction history can be recovered just from the paper key.

![screenshots](/images/brd-hero-mockup.png)

### Features

- [Simplified payment verification](https://github.com/bitcoin/bips/blob/master/bip-0037.mediawiki) for fast mobile performance
- No server to get hacked or go down
- Single paper key is all that's needed to backup your wallet
- Private keys never leave your device
- Save a memo for each transaction (off-chain)
- Supports importing [password protected](https://github.com/bitcoin/bips/blob/master/bip-0038.mediawiki) paper wallets
- Supports ["Payment protocol"](https://github.com/bitcoin/bips/blob/master/bip-0070.mediawiki) payee identity certification

### Localization

**BRD** is available in the following languages:

- Chinese (Simplified and traditional)
- Danish
- Dutch
- English
- French
- German
- Italian
- Japanese
- Korean
- Portuguese
- Russian
- Spanish
- Swedish

We manage all translations with:

[PhraseApp - Start localizing software the simple way](https://phraseapp.com)

### Building and running

You will need [Xcode](https://developer.apple.com/xcode/) to build and run this app.

Once you have Xcode installed, clone this repository.  Update its submodules by running the following command from the root of your project:

`$ git submodule update --init --recursive`

 Then use Xcode to open the `breadwallet.xcworkspace` file.  From there, you can build and run via the Xcode menu.

### WARNING:

***Installation on jailbroken devices is strongly discouraged.***

Any jailbreak app can grant itself access to every other app's keychain data. This means it can access your wallet and steal your bitcoin by self-signing as described [here](http://www.saurik.com/id/8) and including `<key>application-identifier</key><string>*</string>` in its .entitlements file.

---

**BRD** is open source and available under the terms of the MIT license.

Source code is available at https://github.com/breadwallet
