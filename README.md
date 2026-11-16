# DeviceLab

A sofa remote for your TV, run from your Android phone.

DeviceLab talks to Android TV and Fire TV devices over ADB on your home
network: a fast remote with a touchpad, casting web videos to the TV,
a queue and library, and one-tap fixes (restart a stuck app, clear caches,
reboot). Samsung (Tizen) and LG (webOS) TVs get a basic remote and DLNA
casting.

**Downloads are on the [Releases](../../releases) page.** This repository holds
only the published APKs; the source is not public.

## Install

1. On your phone, download the latest `DeviceLab-x.y.apk` from Releases and
   open it. Allow installing from your browser if Android asks.
2. Open DeviceLab. The setup guide walks you through finding your TV.

Requirements: Android 8.0 or later on the phone; the phone and TV on the same
Wi-Fi network.

## Preparing the TV

- **Fire TV / Android TV:** turn on Developer options, then
  **ADB debugging** (on Fire TV: Settings › My Fire TV › Developer options).
  The first time DeviceLab connects, the TV asks you to allow the phone -
  tick "Always allow" and accept.
- DeviceLab can install its own player app on the TV over ADB, and
  [SmartTube](https://github.com/yuliskov/SmartTube) for YouTube links where
  the TV supports it.
- **Samsung / LG:** no setup on the TV beyond accepting the pairing prompt.
  These are less tested than Fire TV.

## Updating

Install the newer APK over the old one; your devices and settings are kept.
DeviceLab updates its player on the TV from the phone.

## Verifying a download

Each release lists the APK's SHA-256. All releases are signed with the same
key, certificate SHA-256:

```
bd:e1:03:56:cb:8b:5e:74:86:89:81:45:32:ac:63:19:2b:fc:32:d1:9e:81:0d:40:c2:45:43:e6:8c:07:97:3e
```

## Notes

- ADB debugging gives any allowed device full control of the TV. Only allow
  phones you own, and turn ADB debugging off if you stop using DeviceLab.
- DeviceLab plays what you point it at. Only cast content you have the right
  to watch.
- Provided as is, with no warranty.
