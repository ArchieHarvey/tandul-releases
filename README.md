# TANDUL releases

Installers for **TANDUL App**, the Windows program that runs on the shop's counter machines (the till and the
admin panel). This page holds only the installer and its update files. TANDUL's source code is not here.

## Install

1. Open the [latest release](https://github.com/ArchieHarvey/tandul-releases/releases/latest) and download
   `TANDUL-Setup.exe`.
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
choices, the version it last ran with (to show "What's new"), a small log of what the app itself did, and, if it ever crashes, a crash dump file. None of these leave the computer. The shop's own pages keep a sign-in session
and a few display preferences (theme, printer) in the app's browser storage, and a receipt being printed is
written to a temporary file that is deleted afterwards.

What the app connects to: the shop's own server, and GitHub to look for and download updates (GitHub can see
the computer's internet address). There is no analytics, tracking or crash reporting, and nothing about your
shop is sent to GitHub.

## Latest release: 1.10.22.12

- Point at the server-speed graph in About to see the time and the response of any check, including ones that got no answer.

## All changes

## 1.10.22.12

- Point at the server-speed graph in About to see the time and the response of any check, including ones that got no answer.

## 1.10.22.11

- The shell now keeps a quiet record of how fast the server has been answering. About opens with the last two minutes already drawn, and Copy diagnostics says when it was slow or did not answer.
- It only checks while the window is showing and the machine is awake, and keeps nothing on disk.

## 1.10.22.9

- The installer now puts TANDUL in a folder called TANDUL, not @tanduldesktop.
- About, Update and Terms windows now step out of the way when you switch to another program, and come back when you return to TANDUL.
- About shows a small line of how fast the server has been answering, and Change server sits under it. Node and system details are gone from the card (Copy diagnostics still has them).
- Terms line says Terms accepted with the version when the day you agreed was never recorded.

## 1.10.22.8

- Clicking an older small window (such as About behind Latest version) now brings it forward and keeps it there, instead of flashing and falling back.
- Closing a small window passes the focus to the next one in front, so the others stay put.
- About says Terms agreed on with the day you agreed. A machine that agreed before the day was recorded shows the version of the terms instead.

## 1.10.22.7

- Change server now opens the setup screen with the address this machine already uses, instead of resetting to the default. The saved address is only replaced once a new one has been checked and works.

## 1.10.22.6

- The browser's developer tools are locked in the installed app, and starting it with a remote-debugging switch is refused.
- In About, the Connected to line is tidier: the speed on the right and the address on its own line, with the reason shown under it when the shop cannot be reached.

## 1.10.22.5

- The small windows now stack properly: a window opened from another stays in front of it, a click on the dimmed till brings forward the right one, and all of them step back when you switch to another program.
- In About, Change server is now a small link next to the address, and the three buttons sit on one row.
- The round marks in the update windows are centred.
- The taskbar and its right-click list now say TANDUL instead of an old description, and the old cached name is cleared once.

## 1.10.22.4

- The setup screen is simpler: choose the till or the admin panel, and a line shows exactly where this machine will connect (for example pos.tandul.in). Click the address to type a different server.
- Connect checks the shop before saving anything, says plainly what went wrong, and no longer leaves a wrong address saved after a failed try.
- The Test connection button is gone, since Connect does the same check.
- On the start-up animation, Click to skip is now plain text, and the dots after Connecting to the shop have more space.

## 1.10.22.3

- If the shop's server is down and answers with an error page (such as a tunnel error), TANDUL shows the reconnecting screen and opens the till again by itself when the server is back.
- When checking for updates fails, the window now says why (no internet, GitHub not answering, update files not ready, or unexpected), with Show details and Copy diagnostics.
- The start-up animation is skipped only by clicking Click to skip (or pressing Esc), not by clicking anywhere.

## 1.10.22.2

- The start-up animation can only be skipped with a click or Esc, Enter or Space, and it runs on real time so it always finishes properly.
- The setup screen has even spacing, with messages shown under the buttons.
- The update window no longer ends the version with a full stop, so it cannot be mistaken for part of the number.
- Windows now calls the program TANDUL in the taskbar list and Task Manager.

## 1.10.22.1

- TANDUL opens with a start-up animation: six flipping letter tiles spell TANDUL while it connects to the shop. Click or press a key to skip it.
- The line under the tiles says what is really happening: starting, connecting, ready, or that the shop cannot be reached yet.
- With Windows set to reduce motion, the letters simply appear.

## 1.10.21.3

- A release found to be bad can be held back from the server, so no till downloads or installs it.
- If an update does not install, TANDUL says so on the next start instead of staying silent.
- An update chosen for 2 AM that was missed because the till was off is installed just after the till is next started.
- If TANDUL crashes, a crash file is saved on this computer only, and the diagnostics say whether the last run ended normally.

## 1.10.21.2

- TANDUL sits on the same line as the close button at the top of the small windows.
- Errors from the till's own screen are written to the diagnostics log on this computer.
- Diagnostics now show the shop's local time and hide the Windows user name and other private details.
- Save diagnostics to a file from About or the tray menu, to send on for support.

## 1.10.21.1

- Versions are now dates: year.month.day.release, such as 1.10.21.1 for the first release of 21 October (year 1 is 2026).
- The What's new window fits its content, so the space above and below stays even however long the list is.

## 1.0.20

- TANDUL opens by itself when Windows starts. Turn it off from the tray menu or the taskbar's right-click list.
- If the page crashes or freezes, TANDUL says what happened and reloads it by itself.
- The offline screen keeps trying and opens the till again as soon as the shop server answers.
- Setup no longer asks for a server address: pick the till or the admin panel. A different address is under a small link, with a Test connection button.
- The window comes back at the same size and place, and the screen stays awake while a shift is open.
- When a receipt does not print, the till says why (offline, out of paper, cover open) with a Retry button.
- The Printers window shows a status light for each printer.
- About shows the terms you agreed to, with a link to read them, and Copy diagnostics for support.

## 1.0.19

- The governing law and jurisdiction clause of the terms of use now names the courts at Kolkata.
- Because the terms changed, TANDUL asks you to agree to them again the next time it starts.
- Declining the terms closes TANDUL cleanly instead of showing an error.

## 1.0.18

- The terms of use open in a window of their own before TANDUL starts, with nothing behind them.
- You have to scroll to the end of the terms before I agree can be pressed, and the terms are laid out with a heading for each section.

## 1.0.17

- A full-screen button in the top bar of the till and the admin panel (F11 still works).
- In full screen the window buttons are hidden and the clock sits at the right edge; in a normal window they no longer overlap it.

## 1.0.16

- In full screen (F11) the top bar's clock and buttons move over to the right edge.
- The orange Returns button in the dark theme matches TANDUL's orange.

## 1.0.15

- Uninstalling TANDUL now also removes its saved settings, so a reinstall starts fresh.
- The till and the admin panel show a Get app button when opened in a Windows browser.

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
