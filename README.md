# Emotiv SDK - Community Edition

Here is the repository to download the latest Emotiv SDK Community Edition, along with code examples and other development tools.
* Supports EPOC (over Emotiv USB dongle)
* Supports Insight and EPOC+ (over BTLE and Emotiv USB dongle)
* Supports Win32/64, Mac, Android, iOS

If you have questions or have knowledge to share, please visit our [forum](https://emotiv.com/forum/) which is the hub for our developer community.

## Table of Contents
1. [Latest Release](#latest-release)
2. [Supported Platforms](#supported-platforms)
3. [Connecting Your Insight](#connecting-your-insight)
4. [API Documentation](#api-documentation)
5. [Known Issues](#known-issues)
6. [Apps and Tools](#apps-and-tools)
7. [Support](#support)

## Latest Release
Version 3.3.0
* Supports saving/loading profile to Emotiv Cloud (see EmotivCloudClient.h)
* New API IEE_GetAverageBandPowers to get average band powers for:
  * theta (4-8 Hz)
  * alpha (8-12 Hz)
  * low-beta (12-16 Hz)
  * high-beta (16-25 Hz)
  * gamma (25-45 Hz)

Coming soon:
* Emotiv SDK for Ubuntu 14.04 64-bit
* EmoComposer for Win32, Mac
* EmoKey for Win32, Mac

## Supported Platforms
* Insight with Bluetooth SMART (Bluetooth 4.0 or Bluetooth Low Energy) connection currently works with the SDK under:
  * Windows 8 or above
  * Windows 7, **only with Bluetooth adaptor that uses Broadcom BCM20702 chipset**
    (recommended one: Plugable USB 2.0 Bluetooth Adapter, http://plugable.com/products/usb-bt4le)
  * Mac OS X 10.10 or above (check if Bluetooth LMP Version is 0x6 from System Report)
  * Android 4.4.3 or above

* Insight with Emotiv Universal USB Receiver currently works with the SDK under:
  * Windows 7 or above
  * Mac OS X 10.8 or above
  * Android 4.4.3 or above

## Connecting Your Insight
* Windows: Turn on Bluetooth on both Insight and PC, then pair your Insight with Windows built-in Bluetooth service first
* Mac, Android and iOS: Turn on Bluetooth on both Insight and Mac/Android device, then start Emotiv app to use (without first pairing)

## API Documentation
The API reference can be found here:

http://emotiv.com/api/3.3.0/

## Known Issues
* Mac SDK may not work with EPOC+ in 256Hz mode over BTLE and USB dongle properly
* EPOC+ motion data may not be accurate with firmware 0x614 over BTLE and USB dongle

## Apps and Tools

#### CPanel
A web-based Emotiv Control Panel:

https://cpanel.emotivinsight.com

Compatible with Insight / EPOC / EPOC+ via:
* BTLE:
  * Windows 8 or above, with Firefox
  * Mac OS X 10.10 or above, with Safari or Firefox
* [Emotiv USB Universal Receiver](https://emotiv.com/store/product_9.html):
  * Windows 7 or above, with Firefox
  * Mac OS X 10.8 or above, with Safari or Firefox

Please follow the instructions to install the Emotiv browser plugin before using the CPanel.

#### Insight App for Android
Requires Android 4.4 or later

https://play.google.com/store/apps/details?id=com.emotiv.insightapp

#### Insight App for iOS
Requires iOS 8.0 or later, **except iOS 8.3/8.4 due to BTLE data transmission limitation in those versions**

https://itunes.apple.com/us/app/emotiv-insight/id1031805596

## Support

Please check out the topic **Insight** on **Emotiv Help Centre**:

https://emotiv.zendesk.com/hc/en-us/categories/200100495-Insight

Our knowledge base is a good source for further reading:

https://emotiv.zendesk.com/hc/en-us
 
Please also visit our [forum](https://emotiv.com/forum/) for bug reports and feature requests.

Happy coding!

The Emotiv Team
