# TANDUL releases

Installers for **TANDUL App**, the Windows program that runs on the shop's counter machines (the till and the
admin panel). This page holds only the installer and its update files. TANDUL's source code is not here.

## Install

1. Open the [latest release](https://github.com/ArchieHarvey/tandul-releases/releases/latest) and download
   `TANDUL-Setup-1.0.14.exe`.
2. Run it. Windows may warn about an "unknown publisher" because the installer is not code-signed yet:
   choose **More info**, then **Run anyway**.
3. When TANDUL opens, enter the shop's server address and choose whether this machine is the till or the
   admin panel.

## Updates

Installed copies find new versions here by themselves, download them quietly, and offer a restart (a notice
in the till, the tray menu, or **Check for updates**). You can also choose to install tonight at 2 AM. A till
is never restarted in the middle of the day on its own.

## Terms and privacy

TANDUL is proprietary software owned by theAscenders. The installer shows the terms before it installs, and
they are in [LICENSE.md](LICENSE.md). Other people's software that it includes is listed in
[THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt).

What the app keeps on the computer: the shop server's address, which portal this machine is, its printer
choices, and the version it last ran with (to show "What's new"). The shop's own pages keep a sign-in session
and a few display preferences (theme, printer) in the app's browser storage, and a receipt being printed is
written to a temporary file that is deleted afterwards.

What the app connects to: the shop's own server, and GitHub to look for and download updates (GitHub can see
the computer's internet address). There is no analytics, tracking or crash reporting, and nothing about your
shop is sent to GitHub.

## Latest release: 1.0.14

- The installer is now one click: it installs straight away and opens TANDUL, with no setup pages.
- The terms of use are shown the first time TANDUL opens, with Agree or Decline.

## All changes

## 1.0.14

- The installer is now one click: it installs straight away and opens TANDUL, with no setup pages.
- The terms of use are shown the first time TANDUL opens, with Agree or Decline.

## 1.0.13

- The installer and uninstaller now have TANDUL's own look instead of the default blue artwork.
- The terms shown at install are updated, and the privacy notes now list exactly what the app keeps and connects to.
- The list of other people's software in the installer now covers every part the app includes.

## 1.0.12

- The installer now shows TANDUL's terms and asks you to agree before it installs.
- The window buttons in the top corner have no background of their own and sit directly on the page.
- The animated dots in the update windows have a little space before them.

## 1.0.11

- The update download screen shows a large percentage, how much has downloaded, and about how long is left, and says you can keep working.
- The update windows have even padding and no longer lose their bottom edge.

## 1.0.10

- The grey Windows title bar is gone: the top bar of the till and the admin panel is the title bar, and the window buttons match the light or dark theme.
- The About window opens in the middle, shows the app version as plain text, and every row looks the same.
- In Windows' list of installed apps TANDUL now shows as just TANDUL, published by theAscenders.

## 1.0.9

- Printers can be set up from the tray menu or About without signing in: receipt printer, paper size, cash drawer and label printer, with a test receipt.
- The You're up to date window shows the big version number and a Check again button.
- TANDUL's windows share one look, with an all-orange TANDUL wordmark, and About fits its content.

## 1.0.8

- Closing About or the update window no longer sends TANDUL to the background.
- The list of changes in the update window has a slim scrollbar and more room before it needs one.

## 1.0.7

- While About or the update window is open, the till behind it is dimmed and can't be clicked by accident.
- Closing these windows keeps TANDUL in front instead of dropping behind another program.
- The update window stays in front of the till, shows animated dots while it works, and has a cleaner checking bar and version arrow.
- TANDUL now has its own icon on the taskbar, Start menu and shortcuts.

## 1.0.6

- TANDUL's own windows now say just TANDUL.
- The update window opens at the right size, and a long list of changes no longer breaks it.
- A change that runs onto a second line is shown as one item in What's new.

## 1.0.5

- A small release to try the new update window: it lists what changed in a clear list.

## 1.0.4

- A redesigned update window: it shows the version you are moving from and to, lists what changed, and fits its content so nothing is cut off.
- The close button in the corner of TANDUL's windows turns red when you point at it.

## 1.0.3

- The About window now shows the App version and the Cloud version separately, and its Updates row reflects the real update status.
- Updating uses the new branded screens end to end.

## 1.0.2

- Updates use TANDUL's own screens: a Check for updates window with a download bar, and a branded "Updating" screen. TANDUL reopens by itself when it is done.
- A small notice tells you when an update is ready, so you can restart between customers. You can also choose to install it tonight at 2 AM.
- After an update, a "What's new" card says what changed.
- The About window has a corner close button.

## 1.0.1

- TANDUL updates itself from the internet: a new version is downloaded quietly and installs when you restart.
- The About window shows the connection, server version and clock, and can copy details for support.

## 1.0.0

- First release of TANDUL for the counter: bills, stock, purchases, returns and Finance.
