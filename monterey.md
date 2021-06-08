# Mac Apps Compatibility - macOS 13.0 Big Sur

Note that most, if not all, compatibility assessments are my own.
I do not take legal responsibility for any of these assessments of compatibility, nor do I guarantee that my assessments are accurate.
My usage may not be the same as your usage, and so I may have missed certain items that you may notice.
These applications' developers may have more updated information on this subject than me.

## Homebrew

- [x] Homebrew - works ~~but developer tools need to be installed beforehand from the Apple Developer More Downloads page instead of through `xcode-select --install`~~ As of developer beta 2, the install script at brew.sh now works. The `xcode-select --install` command is still slow if run manually, but I can’t tell if that is just slow or actually not working.

## Core Applications

- [ ] Google Chrome
- [ ] 1Password
- [ ] Telegram (App Store version)
- [ ] Facebook Messenger
- [ ] Discord
- [ ] TickTick (App Store Version)
- [ ] Microsoft Word (App Store version)
- [ ] Microsoft Excel (App Store version)
- [ ] Microsoft PowerPoint (App Store version)
- [ ] Notability (App Store)
- [ ] Debit & Credit (App Store)
- [ ] Visual Studio Code
- [ ] VMware Fusion
- [ ] Spotify
- [ ] Insync
- [x] Alfred 4 - works as far as I can tell, though Steven reported issues (I did not)
- [ ] BetterTouchTool
- [ ] Karabiner Elements
- [ ] Logitech Options
- [ ] Degoogled Chromium (Eloston)
- [ ] Carbon Copy Cloner
- [ ] GPG Suite
- [ ] Amphetamine (App Store)
- [ ] Zoom
- [ ] Java 11 JDK
- [ ] Dropbox
- [ ] MEGASync
- [ ] OneDrive (App Store version)
- [ ] Slack

## Other Applications

- [ ] HandBrake - opens, encoding from `.mkv` works
- [ ] Windscribe
- [ ] Bartender - new Bartender 4 beta works
- [ ] MacTeX (CLI Only)
- [ ] TeX Live Utility
- [ ] Minecraft
- [ ] JDownloader
- [ ] RescueTime
- [ ] Keka
- [ ] GIMP
- [ ] Android File Transfer
- [ ] IINA
- [ ] Notion
- [ ] Hex Fiend (App Store version)
- [ ] Macs Fan Control - did not test setting fan profiles as I do not have the paid version
- [ ] MakeMKV - launches, was unable to test any ripping functionality at the moment
- [ ] Transmission
- [ ] Tuxera NTFS - As of Big Sur Beta 2, activation now works. Filesystem appears to function after a reboot to enable kexts (without disabling System Integrity Protection).
- [ ] YAC Reader
- [ ] IntelliJ IDEA
- [ ] Logitech Camera Settings
- [ ] NordVPN
- [ ] The Unarchiver (App Store version)
- [ ] MonitorControl
- [ ] Skype
- [ ] AppCleaner
- [ ] Firefox
- [ ] Cisco AnyConnect
- [ ] Microsoft OneNote (App Store version)
- [ ] Adobe Digital Editions
- [ ] Docker
- [ ] Ghidra
- [ ] Microsoft Edge
- [ ] Postman
- [ ] Steam
- [ ] Wireshark
- [ ] Apple Configurator 2 (App Store)
- [ ] iMovie (App Store)

## Printer Driver

- [ ] Brother MFC-L2700DW

## Command Line Utilities Installed via `brew`

I only tested if these installed, in most cases. Any other testing I do will be indicated.

- [ ] `coreutils`
- [ ] `diff-so-fancy`
- [ ] `git`
- [ ] `mas`
- [ ] `neofetch` - installs and works but does not get status like memory and uptime
- [ ] `nmap`
- [ ] `python`
- [ ] `speedtest-cli`
- [ ] `trash`
- [ ] `tree`
- [ ] `wget`
- [ ] `brew-cask-upgrade` tap (`brew tap buo/cask-upgrade` for `brew cu` command)
