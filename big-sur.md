# Mac Apps Compatibility - macOS 11.0/10.16 Big Sur

Note that most, if not all, compatibility assessments are my own.
I do not take legal responsibility for any of these assesments of compatibility, nor do I guarantee that my assessments are accurate.
My usage may not be the same as your usage, and so I may have missed certain items that you may notice.
These applications' developers may have more updated information on this subject than me.

## Homebrew

- [x] Homebrew - works but developer tools need to be installed beforehand from the Apple Developer More Downloads page instead of through `xcode-select --install`

## Core Applications

- [x] Microsoft Edge
- [x] 1Password
- [x] Telegram
- [x] Caprine
- [x] YakYak
- [x] Discord
- [x] TickTick
- [x] Microsoft Word (App Store version)
- [x] Microsoft Excel (App Store version)
- [x] Microsoft PowerPoint (App Store version)
- [x] Microsoft OneNote (App Store version)
- [x] Notability (App Store) - worked but syncing large amounts of notes from iCloud seems to make it hang. Sometimes it makes progress, sometimes not and I have to force quit it.
- [x] Debit & Credit (App Store)
- [x] Visual Studio Code
- [ ] VMware Fusion - reported not to work by MacRumors Forums, but I have not tested myself. Suspected due to kext changes in Big Sur.
- [x] Spotify
- [ ] Insync - terminates on launch
- [ ] Alfred 4 - testing skipped for now
- [x] BetterTouchTool
- [ ] Karabiner Elements - reported not to work on GitHub repository due to changes in kexts. My testing confirms this.
- [x] Logitech Options
- [x] Google Chrome
- [ ] Carbon Copy Cloner - launches but file copy tasks do not copy over the files that have changed
- [x] GPG Suite
- [x] Amphetamine (App Store)
- [ ] Zoom - reported broken by MacRumors Forums, not tested yet
- [x] Java 11 JDK - works but you need to do the link that allows the system Java wrappers to find the JDK (explained at the end of the `brew` install messages when you install the JDK by running `brew install java11`).
- [ ] Dropbox - reported broken by MacRumors Forums, not tested yet
- [ ] MEGASync
- [ ] OneDrive

## Other Applications

- [x] HandBrake - opens, did not test encoding since I do not have a file to test with at the moment
- [x] Windscribe
- [ ] Bartender - reportedly broken according to MacRumors Forums, have not tested myself yet
- [x] MacTeX
- [x] TeX Live Utility
- [x] Minecraft - launches, did not thoroughly test gameplay
- [x] JDownloader
- [x] RescueTime
- [x] Keka - works, including helper utility to set Keka as default extraction application
- [ ] GIMP - asks for Developer Requisition Access but afterwards is unresponsive and fails to launch
- [x] Itsycal - works, but cannot remove built in macOS menu bar clock due to macOS Big Sur integrating the clock and Notification center
- [x] Android File Transfer - works after manually granting Full Disk Access in Security & Privacy preference pane (the application will not prompt for access)
- [ ] IINA
- [ ] Notion
- [ ] Hex Fiend (App Store version)
- [ ] Macs Fan Control
- [ ] MakeMKV
- [ ] VNC Server
- [ ] Cascadea (App Store)
- [ ] Transmission
- [ ] Suspicious Package
- [ ] Docker Desktop
- [ ] Tuxera NTFS
- [ ] Intel Power Gadget
- [ ] YAC Reader
- [ ] IntelliJ IDEA
- [ ] Dark Reader for Safari (App Store version)
- [ ] Logitech Camera Settings
- [ ] Tunnelblick
- [ ] NordVPN IKE (App Store)
- [ ] The Unarchiver
- [ ] MonitorControl
- [ ] Skype
- [ ] Android Studio
- [ ] Facebook Messenger (App Store version)
- [ ] GitKraken
- [ ] AppCleaner
- [ ] Firefox
- [ ] Postman
- [ ] Adguard for Safari (App Store version)
- [ ] VNC Viewer
- [ ] MongoDB Compass
