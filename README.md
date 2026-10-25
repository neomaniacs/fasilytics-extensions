# FASilytics browser extensions

Free browser extensions for tracking and analytics QA, made by [FASilytics](https://www.fasilytics.fr).
They are not on the Chrome Web Store: each folder holds a ready-to-install zip, its SHA-256 checksum and the install steps.

| Extension | What it does | Browsers | Download |
|---|---|---|---|
| **Tag Inspector** 1.0.1 | Adds a **TagSpy** panel to DevTools that lists every analytics and ads call fired by the page in real time: GA4, Meta, TikTok, Floodlight, Criteo and 14 vendors built-in, plus dataLayer pushes (GTM, tc_vars, digitalData…), with each call's parameters decoded. A ChatGPT button copies a ready-made prompt with all the parameters and opens ChatGPT in a new tab, for a sanity check. | Chrome, Firefox | [tag-inspector/](tag-inspector/) |
| **Console Inspector** 0.5.0 | Adds a **Console Triage** panel to DevTools that turns the console into a short, prioritized to-do list (critical / high / medium / low), each entry with a one-line action. Rule-based: no AI, no key, works offline. A "Copy for AI" button turns a single entry into a ready-to-paste prompt. | Chrome | [console-inspector/](console-inspector/) |
| **Tech Inspector** 0.1.0 | Toolbar popup that lists the technologies of a page **with their identifiers**: CMS, e-commerce platform, tag managers, analytics, ad pixels, consent tools, libraries; container IDs, property IDs, pixel IDs, site keys. Each row shows where the evidence came from (DOM, JS global, network request, cookie, response header). 7,600+ technologies from [enthec/webappanalyzer](https://github.com/enthec/webappanalyzer). | Chrome, Firefox | [tech-inspector/](tech-inspector/) |

## Privacy

None of these extensions sends data to a server: everything is read and shown locally, in your browser.
The permissions they ask for are used only to read the page you inspect (its requests, scripts and, for Tech Inspector, its cookies).

## Verify a download

```bash
cd tag-inspector
shasum -a 256 -c SHA256SUMS
```

## Licence

Tech Inspector is GPL-3.0 (see [tech-inspector/LICENSE](tech-inspector/LICENSE) and [NOTICE](tech-inspector/NOTICE)), because its fingerprint data comes from a GPL-3.0 project. Tag Inspector and Console Inspector: © FASilytics, all rights reserved, free to install and use.

Questions or bugs: trackme@fasilytics.fr
