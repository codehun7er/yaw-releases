# yaw releases

Distribution channel for [yaw](https://github.com/codehun7er/yaw), a local-first
macOS dictation app. Sources live in the (private) main repo; this repo carries
only what an installed copy needs to update itself:

- **[Releases](../../releases)** — signed `yaw-X.Y.Z.zip` bundles. Unzip into
  `/Applications` to install.
- **`appcast.xml`** — the [Sparkle](https://sparkle-project.org) feed installed
  copies poll. Each entry carries an EdDSA signature; the app verifies it against
  the public key baked into its Info.plist before installing anything.
