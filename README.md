# Citadel Server Manager — releases

The Windows app that installs, configures and operates DayZ dedicated servers
from the machine that hosts them: SteamCMD deploys, Workshop mods,
`serverDZ.cfg`, RCON, a live map, scheduled restarts, backups and bans.

**This repo carries the installers and the auto-update feed. The source is private.**

This app runs on a VPS or dedicated box you control. It will not run on a
rented host (Nitrado, GPORTAL, Vykix). For those, use
<https://citadel-hub.com/hosts>: one workshop mod and one file. No Windows app.

## Download

Grab `CitadelSetup-x.x.x.exe` from [the latest release](https://github.com/Sk3tch-Dev-Ux/citadel-server-manager-releases/releases/latest).

1. Run the installer **as Administrator** — it needs that for the Windows
   Firewall rules and to register the Windows Service.
2. Open <http://localhost:3001> to start the setup wizard.

Installed copies check this repo for updates on their own, so you only download
by hand once.

The current installer is **v2.49.2**. Source on git `main` already bounces a
rented-host operator to `/hosts` in the wizard. That bounce is not in this
exe. Cut **v2.49.3** from a Windows box before expecting that screen in the
download. Do not build the installer from Linux.

## Buy a licence

<https://citadel-hub.com/server-manager> — $19.99, one payment, updates included.

Checkout returns you to a page holding your licence key and this download. That
page is bookmarkable and always shows the same key.

## Requirements

| | |
|---|---|
| OS | Windows 10 or later |
| Rented host (Nitrado, GPORTAL, Vykix) | Will not run. Use <https://citadel-hub.com/hosts> |
| Privileges | Administrator |
| DayZ server | An existing dedicated server, or deploy one from the UI |
| SteamCMD | Needed for mod installs and deploys; the wizard configures it |
| Node.js | Bundled with the installer |

In-game admin actions (heal, teleport, spawn, vehicle and world actions) also
need the `@CitadelAdmin` server-side mod. Everything else works without it.

## Support

Ask Citadel at <https://app.citadel-hub.com/support>. Quote the licence id from
your claim page — it is your proof of purchase. There is no Discord ticket
panel.
