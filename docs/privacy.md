---
layout: default
title: Privacy Policy — Meshcore Scanner
permalink: /privacy
---

# Privacy Policy — Meshcore Scanner

_Last updated: 2026-04-18_

Meshcore Scanner ("the app") is an iOS application that connects to a MeshCore
BLE companion radio and logs LoRa repeater discoveries to a map. This document
describes how the app handles your data.

## 1. Data we process

The app processes the following data **strictly on your device**:

- **Bluetooth:** the app communicates with a paired MeshCore companion over BLE
  to send discovery requests and receive radio responses.
- **Location (GPS):** while a scan session is active, the app records your
  device's GPS position so that each discovery can be tagged with the location
  where it was received. Background location is used only while a scan session
  is running, to continue logging when the screen is off.
- **Scan results:** timestamps, pseudonymous repeater public-key prefixes,
  signal metrics (SNR, RSSI), and the coordinates where each scan was made.

## 2. How the data is stored

All data is stored **locally on your device**, in the app's private Documents
directory, as plain JSON files (scans, sessions, GPS track, known repeaters,
settings). The data is included in your device's local and iCloud device
backups under your Apple ID, according to your iOS backup settings.

## 3. Data we do not collect

- We do **not** send, upload, sync, or transmit any of your data to our
  servers or to any third party. The app has no backend.
- We do **not** use analytics, advertising, tracking, or crash-reporting SDKs.
- We do **not** use cookies or any form of cross-app or cross-site tracking.
- We do **not** collect any personal identifiers (name, email, phone number,
  Apple ID, advertising identifier, etc.).

## 4. Sharing

The app offers an optional GeoJSON export feature. If you choose to export and
share the file using iOS's standard share sheet, the sharing destination is
entirely under your control; the app itself does not upload anything.

## 5. Permissions

- **Bluetooth:** required to communicate with the MeshCore companion radio.
- **Location (When In Use / Always):** required to tag each scan with GPS
  coordinates. "Always" is used so that GPS logging can continue while a scan
  session runs in the background.

You can revoke these permissions at any time in iOS Settings; the app will
stop recording the corresponding data.

## 6. Children

The app is not directed at children under 13 and does not knowingly collect
any personal data from children.

## 7. Data retention and deletion

All data remains on your device until you delete it. You can remove all stored
data from within the app ("Clear Data" in Settings) or by uninstalling the app,
which removes its entire sandbox.

## 8. Changes to this policy

We may update this policy from time to time. The "Last updated" date at the
top of this document reflects the latest revision.

## 9. Contact

For questions about this policy, contact: **itkeny@gmail.com**

You can also report issues or ask questions at:
[github.com/itk80/MeshcoreScanner/issues](https://github.com/itk80/MeshcoreScanner/issues).
