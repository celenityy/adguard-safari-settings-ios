# adguard-safari-settings-ios

My recommendations for the ultimate configuration of AdGuard on Safari on iOS :)

**NOTE:** This project can be found on both [Codeberg](https://codeberg.org/celenity/adguard-safari-settings-macos), which will act as the main & preferred way to contribute, and [GitHub](https://github.com/celenityy/adguard-safari-settings-macos).

**NOTE:** This is specifically tailored for AdGuard on Safari on iOS. For Safari on macOS, see [here](https://codeberg.org/celenity/adguard-safari-settings-macos), & for AdGuard's extension on other platforms, see [here](https://codeberg.org/celenity/adguard-extension-settings).

**Make sure to set the following under Safari's settings to ensure AdGuard can work at full capacity:**

General -> Extensions:

* AdGuard -> **Allow Extension** -> ✅

* AdGuard -> **Allow in Private Browsing** -> ✅

* AdGuard -> Permissions -> **All Websites** -> `Allow`

* AdGuard - Custom -> **Allow Extension** -> ✅

* AdGuard - Custom -> **Allow in Private Browsing** -> ✅

* AdGuard - General -> **Allow Extension** -> ✅

* AdGuard - General -> **Allow in Private Browsing** -> ✅

* AdGuard - Other -> **Allow Extension** -> ✅

* AdGuard - Other -> **Allow in Private Browsing** -> ✅

* AdGuard - Privacy -> **Allow Extension** -> ✅

* AdGuard - Privacy -> **Allow in Private Browsing** -> ✅

* AdGuard - Security -> **Allow Extension** -> ✅

* AdGuard - Security -> **Allow in Private Browsing** -> ✅

* AdGuard - Social -> **Allow Extension** -> ✅

* AdGuard - Social -> **Allow in Private Browsing** -> ✅

<br>

Settings for Websites -> Content Blockers -> **Use Content Blockers On** -> `All Websites`

Now we can get to the AdGuard :p

# Home

**Protection is on** -> `Safari Protection is on` ✅ 

# Protection

Safari Protection:

Filters:

Off to a fun start, straight to the lists. I would generally recommend enabling most of the built-in filters, besides those under the `Language-specific` category & some of those under the `Other` category. These are all extremely carefully picked lists with strong coverage and minimal breakage, and I would recommend enabling them as follows for the best coverage possible.

**Ad Blocking** -> ✅

Ad Blocking:

* `AdGuard Base filter` -> ✅

* `AdGuard Mobile Ads filter` -> ✅

* `EasyList` -> ✅

<br>

**Privacy** -> ✅

Privacy:

* `AdGuard Tracking Protection filter` -> ✅

* `EasyPrivacy` -> ✅

* `Fanboy's Enhanced Tracking List` -> ✅

* `Peter Lowe's Blocklist` -> ✅

* `Fanboy's Anti-Facebook List` -> ✅

* `Fanboy's Anti-thirdparty Fonts` -> ✅

<br>

**Social Widgets** -> ✅

Social Widgets:

* `AdGuard Social Media filter` -> ✅

* `Fanboy's Social Blocking List` -> ✅

<br>

**Annoyances** -> ✅

Annoyances:

* `AdGuard Annoyances filter` -> ✅

* `AdGuard Cookie Notices filter` -> ✅

* `AdGuard Popups filter` -> ✅

* `AdGuard Mobile App Banners filter` -> ✅

* `AdGuard Other Annoyances filter` -> ✅

* `AdGuard Widgets filter` -> ✅

* `Adblock Warning Removal List` -> ✅

* `Fanboy's Annoyances` -> ✅

* `I don't care about cookies` -> ❌ *(Company behind this list ([Avast](https://wikipedia.org/wiki/Avast)) is sketchy and known for selling data. Adding the list here is *probably* harmless, but I don't see any reason to since AdGuard & EasyList Cookie are already effective at removing cookie banners and enabling them already puts us on par with what uBlock Origin includes, so I'd rather stay safe than sorry here)*

* `EasyList Cookie List` -> ✅

* `Dandelion Sprout's Annoyances List` -> ✅

<br>

**Security** -> ✅ *(Sadly paid, but if you did pay then there's no reason not to enable it & any filter lists in here)*

**Other** -> ✅

Other:

`AdGuard DNS filter` -> ✅ *(Only enable this if you don't also have DNS content blocking with this list enabled in place, otherwise keep this list disabled and re-disable the `Other` category)*

<br>

**Custom** -> ✅ *(Sadly paid, but if you did pay then there's no reason not to take advantage of this)*

Custom:

**NOTE:** Due to unfortunate limitations from Apple, we can only add up to 150,000 rules here. This means we have to be careful with what we add, which is why you'll see some smaller & more optimized lists here vs. more comprehensive protection like I usually recommend. This is also a great example of one of the many reasons why it's important to have a good DNS content blocker (see `Additional recommendations` below), so we don't have to rely on the extension when unnecessary.

I would recommend adding the following custom filters:

* ⭐️ Divested Fingerprinting Blocklist: `https://codeberg.org/divested/dnsbl/raw/branch/master/Fingerprinting.ubl`

* ⭐️ Yokoffing's `Block third party fonts` - `https://raw.githubusercontent.com/yokoffing/filterlists/main/block_third_party_fonts.txt`

Additionally, if you don't have a DNS content blocking solution in place *(you should)*, or you just can't use the relevant list on your DNS blocker, you should import the following:

⭐️ Amnesty International Investigations Blocklist - `https://codeberg.org/divested/dnsbl/raw/branch/master/Amnesty.txt`

⭐️ Dandelion Sprout's Anti-Malware List: `https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt`

⭐️ Disconnect Blocklist - `https://codeberg.org/divested/dnsbl/raw/branch/master/Disconnect.txt`

⭐️ HaGeZi's Badware Host Blocking: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/hoster.txt`

⭐️ HaGeZi's Dynamic DNS Blocking: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/dyndns.txt`

⭐️ HaGeZi's Most Abused TLDs: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/spam-tlds.txt`

⭐️ HaGeZi's Multi PRO++ mini: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/pro.plus.mini.txt`

⭐️ HaGeZi's Pop-Up Ads: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/popupads.txt`

⭐️ OISD - Small: `https://small.oisd.nl`

Additionally, if you're fine with a little breakage, I would highly recommend:

⭐️ HaGeZi's Multi **Ultimate** mini instead of HaGeZi's Multi **Pro++** mini: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/ultimate.mini.txt`

<br>

User rules:

* **Enabled** -> ✅

*3 dots on top right corner*: -> `Open editor`:

This is where it can really depend on you and your set-up. I'll provide my recommendations and filters here I myself use below:

First, I would highly recommend setting the following to protect against [IDN Homograph attacks](https://wikipedia.org/wiki/IDN_homograph_attack) *You don't need to set this if your DNS provider already provides IDN Homograph Attacks Protection (i.e. NextDNS)*:

* `xn--*`

* `xn--*$doc,popup,frame`

I usually also set the following to always enforce blocking Google's Doubleclick & Google Analytics: ((Why?)[https://github.com/gorhill/uBlock/wiki/Privacy-stuff])

* `||doubleclick.net^$important`

* `||google-analytics.com^$important`

Additionally, I set the following to block social media tracking on websites:

* `||facebook.com^$important,third-party`

* `||facebook.net^$important,third-party`

* `||linkedin.com^$important,third-party`

* `||instagram.com^$important,third-party`

* `||tiktok.com^$important,third-party`

I also set this to block [tracking from Gravatar](https://github.com/gorhill/uBlock/wiki/Privacy-stuff):

* `||gravatar.com^$important,third-party`

I also set these rules to block 3rd party sign-in prompts from Google & Apple, as they're 1: annoying and 2: a tracking concern:

* `||accounts.google.com^$third-party`

* `||appleid.apple.com^$third-party`

* `||appleid.cdn-apple.com^$third-party`

* `@@||accounts.google.com^$domain=youtube.com|chromium.org|gstatic.com|googleusercontent.com`

* `@@||appleid.apple.com^$domain=appleid.cdn-apple.com`

* `@@||appleid.cdn-apple.com^$domain=appleid.apple.com`

Finally, I usually set the following to block the annoying banner on Old Reddit promoting Reddit's new UI.

* `www.reddit.com###redesign-beta-optin-btn`

* `old.reddit.com###redesign-beta-optin-btn`

Once you are done here, make sure to select `Save`.

# Settings

**Auto-Update over Wi-Fi only** -> ❌

**Advanced mode** -> ✅

**Show status bar** -> ✅

Advanced settings -> **Debug logs** -> ❌

Advanced settings -> Low-level settings -> **Background app refresh interval** -> `Every hour` *(If this causes you any issues, you can go down to `Every 3 hours` or `Every 12 hours`)*

# Additional recommendations

* Follow my recommendations for iOS [here](https://codeberg.org/celenity/ios-settings). *(See Safari specificially [here](https://codeberg.org/celenity/ios-settings#safari))*.

* Use a private, secure, & reputable DNS provider of your choice. I would recommend setting up your own [NextDNS](https://nextdns.io) configuration if you are able to *(See my recommendations for NextDNS [here](https://codeberg.org/celenity/nextdns-settings))*, otherwise I would recommend [Quad9](https://quad9.net/).

* Enable [Lockdown Mode](https://support.apple.com/105120).

* Enable Safari's [Fraudulent Website Warning](https://www.apple.com/legal/privacy/data/en/safari/).

* Use a (reputable) VPN. I would generally recommend either [Mullvad](https://mullvad.net/), [IVPN](https://www.ivpn.net/), or [ProtonVPN](https://protonvpn.com/).
