# Mac Apps Compatibility - macOS 12.0 Monterey

Note that most, if not all, compatibility assessments are my own.
I do not take legal responsibility for any of these assessments of compatibility, nor do I guarantee that my assessments are accurate.
My usage may not be the same as your usage, and so I may have missed certain items that you may notice.
These applications' developers may have more updated information on this subject than me.

## Homebrew

- [x] Homebrew - installs fine (unlike last year) after `xcode-select --install`, Casks install fine

## Core Applications

- [x] Google Chrome
- [x] 1Password
- [x] Telegram (App Store version)
- [x] Facebook Messenger
- [x] Discord - new audio in screen share feature does not work (relies on Rogue Amoeba ACE, works on Big Sur)
- [x] TickTick (App Store Version)
- [x] Microsoft Word (App Store version)
- [x] Microsoft Excel (App Store version)
- [x] Microsoft PowerPoint (App Store version)
- [x] Notability (App Store)
- [x] Debit & Credit (App Store)
- [x] Visual Studio Code
- [x] VMware Fusion
- [x] Spotify
- [x] Insync
- [x] Alfred 4 - works as far as I can tell, though Steven reported issues (I did not)
- [x] BetterTouchTool
- [x] Karabiner Elements
- [x] Logitech Options
- [x] Degoogled Chromium (Eloston)
- [x] Carbon Copy Cloner
- [x] GPG Suite - Mail extension is reporteddly broken but I don't use that
- [x] Amphetamine (App Store)
- [x] Zoom
- [x] Java 11 JDK - `brew` does not support installing bottles for MacOS 12 just yet
- [x] Dropbox
- [x] MEGASync
- [x] OneDrive (App Store version)
- [x] Slack

## Other Applications

- [x] HandBrake
- [x] Windscribe
- [ ] Bartender - installs, but the features I use are broken (developer is working on fixes)
- [x] MacTeX (CLI Only)
- [ ] TeX Live Utility - attemtping to use the Actions menu to do updates is broken and crashes the application
- [x] Minecraft
- [x] JDownloader
- [x] RescueTime
- [x] Keka
- [x] GIMP
- [x] Android File Transfer
- [x] IINA
- [x] Notion
- [x] Hex Fiend (App Store version)
- [x] Macs Fan Control
- [ ] MakeMKV - crashed on launch but I also had no optical drives connected, so that could be why
- [x] Transmission
- [x] Tuxera NTFS
- [x] YAC Reader
- [x] IntelliJ IDEA
- [ ] Logitech Camera Settings - no camera detected (the camera itself works fine, just not the app)
- [x] NordVPN
- [x] The Unarchiver (App Store version)
- [x] MonitorControl
- [x] Skype
- [x] AppCleaner
- [x] Firefox
- [x] Cisco AnyConnect
- [x] Microsoft OneNote (App Store version)
- [x] Adobe Digital Editions
- [x] Docker
- [x] Microsoft Edge
- [x] Postman
- [x] Steam - Steam itself runs, but I did not test my games
- [x] Wireshark
- [x] iMovie (App Store)

## Printer Driver

- [ ] Brother MFC-L2700DW

## Command Line Utilities Installed via `brew`

I only tested if these installed, in most cases. Any other testing I do will be indicated.

- [x] `coreutils`
- [x] `diff-so-fancy`
- [x] `git`
- [x] `mas`
- [x] `neofetch`
- [x] `nmap`
- [x] `node`
- [x] `python`
- [x] `speedtest-cli`
- [x] `trash`
- [x] `wget`
- [x] `brew-cask-upgrade` tap (`brew tap buo/cask-upgrade` for `brew cu` command)
