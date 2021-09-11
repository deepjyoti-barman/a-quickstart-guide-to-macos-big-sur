# A Quickstart Guide to MacOS Big Sur

## First things to check after purchase

- You are connected to your apple id.
- Your fingerprint has been recorded and registered with 'Touch ID' for easier unlocks and purchases on your Mac.
- Your voice has been recorded and registered with 'Siri'.
- Updates from 'App Store' and 'Software Update' has been successfully installed if available.
- Backup of your system has been taken by 'Time Machine'.

## Applications to install

- AnyDesk
- Apache JMeter
- Apache Maven
- AppCleaner
- Charles
- DBeaver Community Edition
- Git
- Google Chrome
- Grammarly
- Homebrew
- IntelliJ IDEA Community Edition
- iTerm2
- Java SE Development Kit 8
- Java SE Development Kit 11
- Microsoft Teams
- Node.js
- Postman
- PyCharm Community Edition
- Python
- Sublime Text
- The Unarchiver
- Visual Studio Code
- Vysor
- WPS Office
- Zoom

## Invert mouse scroll direction

Click on the `Apple` menu -> Go to `System Preferences` -> `Mouse` -> Untick `Scroll direction: Natural`.

## Display all sidebar items in Finder

Open up `Finder` -> Click on `Finder` in the menu bar -> `Preferences` -> `Sidebar` -> Check all possible items you want to show on the sidebar.

## Changing workspace

- Swipe left or right with three or four fingers on trackpad.
- Swipe left or right with two fingers on magic mouse.
- `Control + Right_Arrow` : To switch to the workspace on the right.
- `Control + Left_Arrow` : To switch to the workspace on the left.
- Open Mission Control by swiping up with three or four fingers to have an overview of all the workspaces running.

## iTerm2 configuration

Open up `iTerm2` -> Click on `iTerm2` in the menu bar -> `Preferences` -> `Profiles`

1. General Tab:  
    - Click on `+` icon to create a profile.  
    - `Name`: `Deepjyoti`
    - `Title`: `Job + Args`
    - Select the newly created profile -> Click on `Other Actions` -> `Set  as Default`
2. Text Tab:
    - Check-in `Blinking Cursor`
    - Set `Font` as the following:  
    `Monaco` `Regular` `10` `100` `110`
    - Uncheck `Anti-aliased`
3. Window Tab:
    - `Transparency`: `17`
    - `Blending`: `50`
    - Settings for Windows:  
    `Columns`: `170`, `Rows`: `40`

## Installing Homebrew on Mac Intel and M1 chip

- Command for Intel chip:  
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

- Command for M1 chip:  
`arch -x86_64 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

## Uninstalling Oracle JDK from Mac

To uninstall / remove Oracle JDK from Mac run the following commands one after another or delete these files and directories manually.

- Removing JDK  
`sudo rm -rf "/Library/Java/JavaVirtualMachines/jdk(version).jdk"`

- Remove Java applet plugin  
`sudo rm -rf "/Library/Internet\ Plug-Ins/JavaAppletPlugin.plugin"`

- Remove Java control panel  
`sudo rm -rf "/Library/PreferencePanes/JavaControlPanel.prefPane"`

- Remove Applet, Web Start and installation related caches  
`sudo rm -rf "~/Library/Application\ Support/Oracle/Java"`  
`sudo rm -rf "/Library/Application\ Support/Oracle/Java"`  
`sudo rm -rf "~/Library/Application\ Support/Java"`

## Resolve ChromeDriver opening failure in Mac

Click on the `Apple` menu -> `System Preferences` -> `System and Security` -> `General` -> Message will be shown as 'ChromeDriver is blocked' -> Click on `Allow Anyway`

## Change Github username and password which are being used from terminal

Recently the Github team has announced that for better protection and privacy users should not use their profile password to push or pull code changes from Github repositories instead they should start using Personal Access Tokens provided by Github. The following process will guide you how to replace your old password with new Personal Access Token generated from your own Github account.

- Check whether credential helper is set or not  
`> git config --list`  
`credential.helper = osxkeychain`

- Update the credentials via Keychain Access  
    1. Open up 'Spotlight Search' by clicking on the icon in the menu bar or pressing `Command + Spacebar`.
    2. Type 'Keychain Access' and press `Enter` to launch the app.
    3. In 'Keychain Access' search for 'github.com'.
    4. Find the 'internet password' entry for 'github.com'.
    5. Edit it by double clicking on it (you may delete it from here as well).
    6. Click on 'Show Password' checkbox.
    7. Enter your login password.
    8. Replace the old password with new Personal Access Token once it's visible.
    9. Save the changes.
    10. Close the application.

- Deleting your credentials via command line.  
`> git credential-osxkeychain erase`  
`host = github.com`  
`protocol = https`  
`> [Return]`

## Shortcuts

- `Command + Space` : Open up 'Spotlight Search' for searching any application, document etc. on your system or on the web.
- `Command + Q` : Quit the currently open application.
- `Command + M` : Minimize the focused window.
- `Command + Shift + 3` : Capture a full size screenshot of the window.
- `Command + Shift + 4` : Capture a portion of the screen.
- `Command + Delete` : __(Finder)__ Move selected items to bin.
- `Command + C` : __(Finder)__ Copy the selected files and directories.
- `Command + V` : __(Finder)__ Paste files and directories that has been copied into the current location.
- `Command + Option + V` : __(Finder)__ Move files and directories that has been copied into the current location.
- `Command + Down_Arrow` : __(Finder)__ Go one level inside the directory hierarchy / open up a file or directory.
- `Command + Up_Arrow` : __(Finder)__ Go one level up in the directory hierarchy.
- `Command + Control + T` : __(Finder)__ Add the currently open directory in the sidebar.
- `Command + Control + S`: __(Finder)__ Show / Hide the sidebar.
- `Command + Shift + .` : __(Finder)__ Show / Hide all the hidden files and directories.
- `Command + S` : __(Text Editor)__ Save documents, files in text editor and IDEs.
- `Command + Shift + Left_Arrow` : __(Text Editor)__ Select text from the cursor location to the beginning of the line.
- `Command + Shift + Right_Arrow` : __(Text Editor)__ Select text from the cursor location to the end of the line.
- `Delete` : __(Text Editor)__ Deletes a single character on the left of the cursor.
- `Fn + Delete` : __(Text Editor)__ Deletes a single character on the right of the cursor.
- `Option + Left_Arrow` : __(Text Editor)__ Move to the beginning of each word on the left.
- `Option + Right_Arrow` : __(Text Editor)__ Move to the end of each word on the right.
- `Control + A` : __(Terminal)__  Move cursor to the beginning of the line.
- `Control + E` : __(Terminal)__ Move cursor to the end of the line.
- `Esc + B` : __(Terminal)__ Move cursor one word forward.
- `Esc + F`: __(Terminal)__  Move cursor one word backward.
- `Control + W` : __(Terminal)__ Delete word on the left.
- `Esc + D` : __(Terminal)__ Delete word on the right.
- `Control + K` : __(Terminal)__ Delete all characters to the right of the cursor.
- `Control + D` : __(Terminal)__ Delete the current character.
- `Control + U` : __(Terminal)__ Delete entire line.
- `Control + C` : __(Terminal)__ Cancel the current command.
- `Control + L` : __(Terminal)__ Clear the terminal screen.
- `Control + R` : __(Terminal)__ Search in previous commands (history).

## Commands

- `sudo shutdown -h now` : Shuts down your system immediately.
- `sudo shutdown -r now` : Restarts your system immediately.
- `open .` : Open the current directory in Finder.
- `ls > ~/Desktop/files.txt` : __(I/O Redirection)__ Redirects the output of 'ls' command to 'files.txt', overwrites the existing content if the file already exists.
- `ls >> ~/Desktop/files.txt` : __(I/O Redirection)__ Redirects the output of 'ls' command to 'files.txt', appends to the existing content if the file already exists.
- `ls | open -fe` : __(I/O Redirection)__ Redirects the output of 'ls' command and opens it in default text editor of the system (i.e. TextEdit).
- `ls | pbcopy` : __(I/O Redirection)__ Redirects the output of 'ls' command to the clipboard.
