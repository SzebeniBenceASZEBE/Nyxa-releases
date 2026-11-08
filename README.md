# Nyxa releases

Nyxa is a free Windows game launcher that brings your **Steam, Epic Games Store, GOG and
Xbox / PC Game Pass** libraries into one view, with playtime, achievements and covers, and
launches your games from the same place. No ads, no analytics, no Nyxa account.

This repository holds the **installers and update packages only**. It contains no source code.
The app checks the releases here for updates.

**Website:** [nyxa.party](https://nyxa.party/)

## Download

Get the **`Setup.exe`** from the [latest release](https://github.com/SzebeniBenceASZEBE/Nyxa-releases/releases/latest)
and run it. No administrator rights are needed: Nyxa installs for your Windows user only.

**Requirements:** Windows 10 or 11, 64-bit, and the Microsoft Edge WebView2 Runtime, which comes
with Windows 11 and is already installed on most Windows 10 PCs.

### "Windows protected your PC"

The installer is not code-signed yet, so Windows SmartScreen does not recognise it. Click
**More info**, then **Run anyway**. Only do this with a file downloaded from this repository's
releases page.

## Updates

Nyxa checks this repository when it starts. When a new version has downloaded, an
**UPDATE READY · RESTART** button appears in the header: click it to update now, or simply close
Nyxa and it installs the update on its way out.

Your library, settings and store sign-ins are stored outside the program folder, so they stay
in place through updates and reinstalls.

## Your data

- Nyxa never sees your store passwords. You sign in on each store's own page.
- Store sign-ins are kept as tokens, encrypted with Windows' own data protection (DPAPI), on
  your PC only.
- Game titles and store IDs go to the Nyxa server (`api.nyxa.party`) to look up covers and
  details on IGDB and SteamGridDB. No account data is sent, and the server does not log your
  IP address.

The full description is on the [website](https://nyxa.party/).

## Uninstalling

Uninstall Nyxa from Windows Settings, under Apps. To remove your data as well, delete these two
folders afterwards:

- `%AppData%\Nyxa` (library database and settings)
- `%LocalAppData%\Nyxa` (sign-ins, covers and the log)

## Feedback and bug reports

Please report problems on [Discord](REPLACE-DISCORD-INVITE). If something went wrong, Nyxa can
export a diagnostics file in Settings, under Diagnostics; attach it to your message. The file is
never sent automatically.

## Source code

The source code will be published in a separate repository: [REPLACE-PUBLIC-REPO-URL](REPLACE-PUBLIC-REPO-URL).

## Licence

© 2026 Szebeni Bence. All rights reserved. No licence has been chosen for Nyxa yet.

Nyxa includes third-party components under their own licences. Their notices
(`THIRD-PARTY-NOTICES.md` and the `licenses` folder) are installed next to the program, and the
About page in Settings opens them.

Game data and covers come from [IGDB](https://www.igdb.com/), artwork from
[SteamGridDB](https://www.steamgriddb.com/).

Nyxa is an independent project, not affiliated with, endorsed or sponsored by Valve, Microsoft,
Epic Games, GOG, IGDB or SteamGridDB. Steam, Xbox, PC Game Pass, Epic Games Store and GOG are
trademarks of their respective owners.
