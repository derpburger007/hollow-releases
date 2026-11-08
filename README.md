# HOLLOW

HOLLOW is a Windows 11 companion app for Deadlock, made by a player. This repository holds its installers and signed update files. The source code isn't published here.

HOLLOW is unofficial and isn't affiliated with or endorsed by Valve.

## What it does

- Tracks match history, win rate, K/D/A and hero stats
- Opens any match to show a souls timeline, key moments, item build and both scoreboards
- Shows player profiles with titles that explain themselves, a ranked chart, the game's own awards and who you play with most
- Lists every hero with a tier, the reason for it, and a short guide
- Follows your match live in a separate Field View window, with both teams' heroes, K/D/A and souls
- Browses heroes and community builds
- Shows the mods you installed with Deadlock Mod Manager, and browses more on GameBanana, if you turn Mods on
- Answers questions about your matches with a local AI model in LM Studio or Ollama
- Shows your last match on your Discord profile, if you turn that on
- Comes with HOLLOW Test Mode, a separate copy filled with made-up matches for trying things out

## Install

Download `HOLLOW_Setup_<version>.exe` from [Releases](../../releases/latest) and run it. You'll need 64-bit Windows 11. The installer adds Microsoft's WebView2 Runtime if it's missing.

The installer isn't code signed, so Windows SmartScreen and antivirus software may warn you. Only run files from this repository's Releases page.

If something isn't working, open Settings, Troubleshooting and choose Run a check. It says what's wrong and how to fix it.

## Privacy

- HOLLOW has no accounts, telemetry, analytics or ads.
- Your settings, match records and chats stay on your PC.
- It reads public match data from the [Deadlock API](https://deadlock-api.com), and Steam's public match broadcast through that API.
- It reads the console.log file Deadlock writes when launched with `-condebug`, to know when you're in a match.
- It never asks for your Steam password.
- It doesn't inject into Deadlock, read its memory, change its files or send it input.
- Mods: it only reads Deadlock Mod Manager's saved list. It never installs, removes or changes mods.
- If you press Alt+F4 in Deadlock, HOLLOW asks the game's window to close, the same request as Close window on the taskbar. You can turn this off in Settings.

## Updates

Update checks are off by default. HOLLOW installs an update only if it's signed with the project's private key and the file matches that signature.

HOLLOW already knows where to look. Choose Check for updates in Settings, Updates, or turn on automatic checks there.
