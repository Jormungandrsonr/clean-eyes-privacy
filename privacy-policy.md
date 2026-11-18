# Clean Eyes privacy policy

*Last updated: 18 November 2026*

Clean Eyes is a content blocker for Windows, Android and the Chrome and Edge browsers. It blocks adult
content and anything on your own list. This page says exactly what it does with your information.

**The short version:** Clean Eyes works on your own device. It does not have accounts, ads or trackers, and it
does not sell or share data. It sends nothing about you to the developer unless you turn on the optional
"Help improve Clean Eyes" setting, which is off until you choose it.

## What stays on your device

- **Your rules and settings** (sites, keywords, exceptions, which packs are on) are stored on your device only.
- **The pages you visit** are looked at on your device so the rules can be applied. The addresses and page titles
  are not sent anywhere. The browser extension needs permission to see pages for this reason.
- **The list of recent blocks** you see in the app is stored on your device and can be cleared.
- **Your buddy's code secret** (the authenticator secret that approves changes) is stored encrypted on your
  device. Clean Eyes has no server that holds it, and the developer cannot see it.

## What Clean Eyes sends over the internet while you use it

These are needed for it to work, and none of them include your rules or a list of what you browse.

- **Block lists.** Clean Eyes downloads public lists of adult websites from GitHub and jsDelivr (the HaGeZi and
  StevenBlack lists). The server that provides a list can see your network address, as with any download.
- **DNS lookups.** The Windows and Android apps check each website name against your rules. Names that are
  allowed are passed on to a DNS provider so the page can load. By default this is **Cloudflare for Families**
  (1.1.1.3), which also filters adult sites, and Cloudflare's privacy policy applies to those lookups. You can
  change this to your network's own DNS in the Windows settings.
- **Reddit communities.** To block only the 18+ parts of Reddit, the extension and the Android app ask
  reddit.com whether a community is marked 18+ (a request for `reddit.com/r/<name>/about.json`, made the same way
  your browser makes any request to Reddit). Reddit can see those requests.

## Optional: Help improve Clean Eyes

There are three levels. The default is **Off**, and nothing is recorded or sent. You choose a level in the
extension's options page, the Windows settings app or the Android app, and you can change it or turn it off at
any time.

| Level | What is sent |
|---|---|
| **Off** | Nothing. |
| **Errors and health** | Error messages and crashes, the app version, your operating system version, and numbers about whether Clean Eyes is working (for example whether the filter is running and how many rules are loaded). No websites. |
| **Test mode** | Everything in the level above, plus the address of each page your browser opens, each page that is blocked and the rule that blocked it, and website names looked up by the filter. This is for people testing the blocker and is not meant for everyday use. |

How it is handled:

- Reports are sent to a small server run by the Clean Eyes developer on Cloudflare (Workers and KV storage). The
  server does not read or store your network address.
- Each device uses a random identifier that is not linked to your name, email or accounts.
- **Errors-and-health reports are deleted automatically after 30 days, and test-mode reports after 14 days.**
- Your rules, the text you type into pages, passwords and your buddy's codes are never included.
- **Delete what you sent.** Each app has a "Delete what this browser (PC, phone) has sent" button, which asks the
  server to delete everything that device sent and starts a new random identifier.
- The reports are used only to find and fix problems in Clean Eyes. They are not sold, shared or used for
  advertising.

## Children and sharing

Clean Eyes is often used by someone together with a "buddy" they trust. The buddy sees only the six-digit codes
from their own authenticator app and any message you choose to send them. Clean Eyes does not send your activity to
your buddy.

## Permissions the extension asks for, and why

| Permission | Why |
|---|---|
| Read and change pages on all websites | To check each page against your rules, to read the adult rating label some sites include, and to hide 18+ posts on Reddit. |
| Tabs and web navigation | To see which address a tab is opening and show the block page instead. |
| Web request | To read the adult rating header some sites send. |
| Declarative net request | To block known pages before they load. |
| Storage and alarms | To keep your rules and refresh them regularly. |

## Contact

Questions or requests about your information: [CONTACT ADDRESS: fill in before publishing].

If this policy changes, the date at the top changes, and any change that sends more information will only take
effect if you choose it.
