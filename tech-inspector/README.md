# FASilytics Tech Inspector — packaged builds

Ready-to-install builds of FASilytics Tech Inspector, built from this repository. Each zip is listed in `SHA256SUMS`.

## Verify the download

```bash
shasum -a 256 -c SHA256SUMS
```

Each line must end with `OK`.

## Install in Chrome (or Edge, Brave, Arc)

The extension is not on the Chrome Web Store, so Chrome installs it in developer mode:

1. Unzip `fasilytics-tech-inspector-0.1.0-chrome.zip` into a folder you will keep (Chrome loads it from there).
2. Open `chrome://extensions`.
3. Turn on **Developer mode** (top right).
4. Click **Load unpacked** and select the unzipped folder.

To update: unzip the new version over the same folder, then click the reload icon on the extension card.

## Install in Firefox

`fasilytics-tech-inspector-0.1.0-firefox.zip` is not signed by Mozilla, so Firefox loads it until the next restart:

1. Unzip it.
2. Open `about:debugging#/runtime/this-firefox`.
3. Click **Load Temporary Add-on…** and select `manifest.json` in the unzipped folder.
