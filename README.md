# Ovis sideload APK

Unofficial Android build of [Ovis](https://github.com/devswha/ovis) for a phone with no Play account. Obtainium can follow the releases in this repository.

This is not the Play build. The package id is `sh.ovis.sideload`, not `sh.ovis.app`, so it does not collide with a later Play install and it is not signed with the maintainer's upload key. Push is off: there is no `google-services.json`, and FCM would not arrive without Play services anyway.

Each release is the latest `devswha/ovis` tag, built as documented in that repo's `docs/native-app.md`, with two edits so Android can update it:

- `applicationId` `sh.ovis.sideload`
- `versionName` set to the upstream tag, and `versionCode` derived from it (`major * 1000000 + minor * 1000 + patch`)

Ovis is MIT, copyright 2026 devswha. The license is in each upstream tag.

## Obtainium

- Source: GitHub
- User / org: `sllrs`
- Repository: `ovis-android`
- Include prereleases: off

The asset is `ovis-sideload-<version>.apk`.
