# Mac Apps Compatibility - macOS 11.0/10.16 Big Sur

Note that most, if not all, compatibility assessments are my own.
I do not take legal responsibility for any of these assesments of compatibility, nor do I guarantee that my assessments are accurate.
My usage may not be the same as your usage, and so I may have missed certain items that you may notice.
These applications' developers may have more updated information on this subject than me.

## Homebrew

- [x] Homebrew - works ~~but developer tools need to be installed beforehand from the Apple Developer More Downloads page instead of through `xcode-select --install`~~ As of developer beta 2, the install script at brew.sh now works. The `xcode-select --install` command is still slow if run manually, but I can’t tell if that is just slow or actually not working.

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
- [ ] VMware Fusion - ~~reported not to work by MacRumors Forums, but I have not tested myself. Suspected due to kext changes in Big Sur.~~ New [tech preview version](https://blogs.vmware.com/teamfusion/2020/07/fusion-big-sur-tech-preview.html) should work, have not tested it yet. Will update status once tested.
- [x] Spotify
- [ ] Insync - terminates on launch. Bug reported on [Insync Forums](https://forums.insynchq.com/t/insync-fails-to-launch-on-macos-big-sur-developer-beta/16186).
- [x] Alfred 4 - works but I can't sync preferences since Insync is broken
- [x] BetterTouchTool
- [ ] Karabiner Elements - reported not to work on GitHub repository due to changes in kexts. My testing confirms this.
- [x] Logitech Options
- [x] Google Chrome
- [x] Carbon Copy Cloner - latest beta works to back up data, enables data-only backups (clones are not bootable without installing macOS onto the backup), see [this Bombich help article](https://bombich.com/kb/ccc5/creating-and-restoring-data-only-backups) for more details.
- [x] GPG Suite
- [x] Amphetamine (App Store)
- [x] Zoom - Version 5.1.1 appears to work now. Graphical issues are fixed. Video is still wonky but that might be a macOS issue, not a Zoom issue, since I've seen similar issues with Photo Booth. This might actually be a "just me" issue since I'm now seeing it on Catalina as well.
- [x] Java 11 JDK - works but you need to do the link that allows the system Java wrappers to find the JDK (explained at the end of the `brew` install messages when you install the JDK by running `brew install java11`).
- [x] Dropbox - beta version 101.3.422 is working on Big Sur, stable is apparently broken. Beta version can be obtained [here](https://www.dropboxforum.com/t5/Dropbox-desktop-client-builds/bd-p/101003016) or with the cask `dropbox-beta`.
- [x] MEGASync
- [x] OneDrive (App Store version) - first initial sync of files is laggy at best and unresponsive at worst until it is done, but that is just OneDrive and not Big Sur (the issue is present in Catalina as well and may just be related to how large my OneDrive is and how many files are in it). Disabling the Files On Demand feature required a force quit of OneDrive to get files to start downloading but it appears to be working just fine now.

## Other Applications

- [x] HandBrake - opens, encoding from `.mkv` works
- [x] Windscribe
- [ ] Bartender - launches and I am able to configure settings, but nothing actually works (no icons are hidden)
- [x] MacTeX
- [x] TeX Live Utility
- [x] Minecraft - launches, did not thoroughly test gameplay
- [x] JDownloader
- [x] RescueTime
- [x] Keka - works, including helper utility to set Keka as default extraction application
- [ ] GIMP - asks for Developer Requisition Access but afterwards is unresponsive and fails to launch
- [x] Itsycal - works, but cannot remove built in macOS menu bar clock due to macOS Big Sur integrating the clock and Notification Center
- [x] Android File Transfer - works after manually granting Full Disk Access in Security & Privacy preference pane (the application will not prompt for access)
- [x] IINA
- [x] Notion
- [x] Hex Fiend (App Store version)
- [x] Macs Fan Control - did not test setting fan profiles as I do not have the paid version
- [x] MakeMKV - launches, was unable to test any ripping functionality at the moment
- [x] Transmission
- [ ] Tuxera NTFS - As of Big Sur Beta 2, activation now works. It remains to be seen whether the filesystem functions or not.
- [x] Intel Power Gadget - works after rebooting to enable the kernel extension for the first time. Unknown if the kernel extension is only working now because Big Sur is still a beta, or if it will continue to work after the public release.
- [x] YAC Reader
- [x] IntelliJ IDEA - only tested barebones functionality - making a project, editing `.java` files,  compiling, and running
- [x] Logitech Camera Settings
- [x] Tunnelblick Beta - both my full and split UDP VPN tunnels appear to work. The application complains that the `/tmp/` folder is insecure but otherwise appears it appears as though it continues to work.
- [x] NordVPN IKE (App Store version)
- [x] The Unarchiver
- [x] MonitorControl - changing brightness via the menubar icon works, did not test keyboard shortcuts since Karabiner Elements is broken at the moment, which is necessary for my keyboard brightness shortcuts to work
- [x] Skype - did not test calling, low priority to do so since Skype is not critically important to me
- [x] AppCleaner
- [x] Firefox
- [ ] Box Sync - terminates on launch (note that I do not use Box Sync on a daily basis so I will probably not revisit this)
- [ ] Google Backup and Sync - terminates on launch
- [ ] Cisco AnyConnect - program installs successfully, but Big Sur blocks the kernel extension from loading and asks for a restart to enable it. Performing the restart does not actually enable the kernel extension and it will repeatedly ask to restart and enable the kernel extension. Supposedly the kernel extension might be possible to enable by disabling System Integrity Protection, but this is a step that (according to [Apple's documentation](https://developer.apple.com/documentation/macos-release-notes/macos-big-sur-11-beta-release-notes)) is only going to work in the betas. Note that the alerts I am seeing could also possibly be related to the fact that kernel extensions included in macOS are alerting as well. Anyways, AnyConnect installs but the VPN itself does not seem to be working. Error during installation states "The VPN client agent was unable to create the client DNS plugin manager".

## Printer Driver

- [x] Brother MFC-L2700DW - must be downloaded manually from [Brother website](https://support.brother.com/g/b/downloadlist.aspx?c=us&lang=en&prod=mfcl2700dw_us_eu_as&os=10060). Download both the Printer Driver and Scanner Driver.

## Command Line Utilities Installed via `brew`

I only tested if these installed, in most cases. Any other testing I do will be indicated.

- [x] `coreutils`
- [x] `diff-so-fancy`
- [x] `git`
- [x] `mas`
- [x] `neofetch` - installs and works but does not get status like memory and uptime
- [x] `nmap`
- [x] `python`
- [x] `speedtest-cli`
- [x] `trash`
- [x] `tree`
- [x] `wget`
- [x] `brew-cask-upgrade` tap (`brew tap buo/cask-upgrade` for `brew cu` command) - tested and appears to work, but I have not tested it when updates are available yet
