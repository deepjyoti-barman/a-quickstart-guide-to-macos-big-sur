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
- Grammarly for Safari
- Homebrew
- IntelliJ IDEA Community Edition
- iTerm2
- Java SE Development Kit 8
- Java SE Development Kit 11
- Katalon Studio
- Microsoft Teams
- Node.js
- Postman
- PyCharm Community Edition
- Python
- Sublime Text
- The Unarchiver
- Visual Studio Code
- Vysor
- XAMPP
- WPS Office
- Zoom

## The necessary Trackpad tweak

- Click on the `Apple` menu -> Go to `System Preferences` -> `Trackpad`
    1. Check `Tap to click`.
    2. Increase tracking speed to 5.

## Invert mouse scroll direction

Click on the `Apple` menu -> Go to `System Preferences` -> `Mouse` -> Untick `Scroll direction: Natural`.

## Display all sidebar items in Finder

Open up 'Finder' -> Click on `Finder` in the menu bar -> `Preferences` -> `Sidebar` -> Check all possible items you want to show on the sidebar.

## Changing workspace

- Swipe left or right with three or four fingers on trackpad.
- Swipe left or right with two fingers on magic mouse.
- `Control + Right_Arrow` : To switch to the workspace on the right.
- `Control + Left_Arrow` : To switch to the workspace on the left.
- Open Mission Control by swiping up with three or four fingers to have an overview of all the workspaces running.

## Reinstall MacOS from MacOS recovery

__Note__: Make sure you have an active internet connection, Mac is plugged into the power / charger and it's turned off.

- Key combinations:
    1. `Command + R`  
    Reinstall the latest version of MacOS installed on your Mac (Recommended for most users).
    2. `Command + Option + R`  
    Upgrade to the latest version of MacOS compatible to your device.
    3. `Command + Option + Shift + R`  
    Reinstall the version of MacOS that came with your Mac.
- Turn on your Mac and immediately press and hold the key combinations of your choice until you see an Apple logo.
- Enter the admin password.
- Click on `Next`.
- Select `Reinstall MacOS` from 'MacOS Utilities'.
- Click on `Continue`.
- Follow the on-screen options.
- When it's done you will see a login window, enter the password and continue with the prompts.

__Tip__: When to do factory reset / reinstall MacOS?  
    - When you are selling your Mac.  
    - Changing admin name.  
    - To fix software issues.  

## Granting Microsoft Teams, Zoom and other softwares resource and device access permissions

Following are the steps to grant 'Microsoft Teams' permission for 'Screen Recording'.

- Click on `Apple` menu -> `System Preferences` -> `Security and Privacy`
- Click on `Privacy` tab.
- Click on `Screen Recording` from the LHS side bar.
- Click on the lock icon to make changes.
- Provide admin password / touch id.
- Click on the checkbox next to 'Microsoft Teams'. If 'Microsoft Teams' is not there as an option then click on the '+' icon and add 'Microsoft Teams' from the Applications folder.
- Click on the unlock icon to lock the changes you have made.
- Close the `Security and Privacy` window.
- Quit 'Microsoft Teams' and reopen it to enact the changes made.

__Tip__: List of necessary permissions for apps,  
    - Microsoft Teams: Accessibility, Camera, Microphone, Screen Recording.  
    - Zoom: Accessibility, Screen Recording.  
    - Terminal: Full Disk Access.  
    - iTerm2: Full Disk Access.

## How to format an external hard disk drive in Mac

__Tip__: In this guide, we're using exFAT instead of FAT32, another filesystem that both Windows and Mac can read and write to, because FAT32 has a maximum 4GB file size limit whereas exFAT can work with files as large as 16EB (exabytes). exFAT also performs better than FAT32.

You can format the drive from either Mac or Windows. However, if you want to use part of the drive for OS X's Time Machine backups, you should do this from the Mac, since there's an extra step to make the drive compatible for Time Machine.

Formatting of the device can be done by following the steps given below:

- Connect an external hard drive to your Mac.
- Open 'Spotlight Search' by pressing `Command + Spacebar`, type in Disk Utility, and click the first option. This will open the Disk Utility app, where you will find all the internal and external drives that are connected to your Mac.
- Choose `View` -> `Show All Devices`
- In the sidebar, select the storage device you want to erase, then click the Erase button.
- Click the Scheme pop-up menu, then choose GUID Partition Map.
- Click the Format pop-up menu, then choose a file system format.
- Enter a name.
- (Optional) If available, click Security Options, use the slider to choose how many times to write over the erased data, then click OK.
[Note: Secure erase options are available only for some types of storage devices. If the Security Options button is not available, Disk Utility cannot perform a secure erase on the storage device.]
- Click Erase, then click Done.

## Terminal configuration

Open up 'Terminal' -> Click on `Terminal` in the menu bar -> `Preferences`

- Select the `General` tab
    1. `On startup, open`: `New window with profile` - `Pro`
    2. `New windows open with`: `Same Profile`

- Select the `Profiles` tab
    1. `Text` tab
        - Select profile `Pro` and click on `Default` button
        - Check `Blink Cursor`
        - Click on `Colors and Effects` -> `Opacity`: `80%`
        - Click on `Change` button next to `Font` -> `Line Spacing`: `1.1`
    2. `Window` tab
        - `Columns`: `170`, `Rows`: `40`

## iTerm2 configuration

Open up 'iTerm2' -> Click on `iTerm2` in the menu bar -> `Preferences` -> `Profiles`

1. General Tab:  
    - Click on `+` icon to create a profile.  
    - `Name`: `Deepjyoti`
    - `Title`: `Job + Args`
    - Select the newly created profile -> Click on `Other Actions` -> `Set  as Default`
    - (Optional) `Send text at start`: `sshpass -e ssh deepjb@192.168.30.15`
2. Text Tab:
    - Check `Blinking Cursor`.
    - Set `Font` as the following:  
    `Monaco` `Regular` `10` `100` `110`
    - Uncheck `Anti-aliased`
3. Window Tab:
    - `Transparency`: `17`
    - `Blending`: `50`
    - `Settings for New Windows`:
    `Columns`: `170`, `Rows`: `40`

## Installing Homebrew on Mac Intel and M1 chip

- Command for Intel chip:  
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

- Command for M1 chip:  
`arch -x86_64 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

## Install and configure tools like Maven / JMeter / Oracle JDK etc. on Mac

- Maven requires Java to execute. So we will have to first install Java and then maven into our Mac OS. Verify the JDK installation by opening the Terminal and run `java -version` command.

- Go to the Maven Download site: <https://maven.apache.org/download.cgi> and download the “Binary tar.gz archive”.

- After downloading, extract it to '/opt' directory using the below command.  
`tar -xvzf apache-maven-3.6.3-bin.tar.gz -C /opt`

- The next step is to set up the environment variables – M2_HOME and Path. We have to add the Maven bin directory to the Path variable.
    1. On macOS 10.5 Catalina or later, the default shell is zsh, and we can create the environment variables MAVEN_HOME and update the PATH in ~/.zshenv. Create .zshenv  and open the it in the default text editor by entering the following command:  
    `touch ~/.zshenv && open ~/.zshenv`

    2. For macOS 10.14 Mojave and before, the default Terminal shell is bash, and we can create the environment variables in ~/.bash_profile. Create .bash_profile and open the it in the default text editor by entering the following command:  
    `touch ~/.bash_profile && open ~/.bash_profile`

- Copy and paste the following content in the .zshenv / .bash_profile and save the changes:

    ```bash
    export M2_HOME=/opt/apache-maven/3.8.2
    export PATH=$PATH:$M2_HOME/bin
    ```

- Source the ~/.zshenv or ~/.bash_profile to reflect the changes.  
    1. `source ~/.zshenv`
    2. `source ~/.bash_profile`

- Finally, run the `mvn -version` command to check if Maven is installed successfully.

__Extras__: My all in one ~/.zshenv config is given below,

```bash
export ANDROID_HOME=/Users/ins667/Library/Android/sdk 
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_301.jdk/Contents/Home
export JMETER_HOME=/opt/apache-jmeter/5.4.1
export M2_HOME=/opt/apache-maven/3.8.2
export SSHPASS='xyz^&12ab&23'

export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/platform-tools
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$JAVA_HOME/bin
export PATH=$PATH:$JMETER_HOME/bin
export PATH=$PATH:$M2_HOME/bin
```

## Installing sshpass - An Excellent Tool for Non-Interactive SSH Login

In most cases, Linux system administrators login to remote Linux servers using SSH either by supplying a password, or passwordless SSH login, or keybased SSH authentication.

sshpass is a simple and lightweight command line tool that enables us to provide password (non-interactive password authentication) to the command prompt itself, so that automated shell scripts can be executed.

### Command to install sshpass in Mac

We can install sshpass using any of the following command:

```bash
brew install hudochenkov/sshpass/sshpass
```
  
```bash
brew install esolitos/ipa/sshpass
```

### 3 ways of login via sshpass

```bash
sshpass -p 'my_pass_here' ssh aaronkilik@10.42.0.1
```

```bash
export SSHPASS='my_pass_here'
sshpass -e ssh aaronkilik@10.42.0.1
```

```bash
sshpass -f password_filename ssh aaronkilik@10.42.0.1
```

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

## Capture a snapshot / record video the entire screen and actions in Mac

- Open up 'Quick Time Player'.
- Click on `File` -> `New Screen Recording`
    1. Select `Capture Entire Screen` option if you want to take a snapshot of the entire screen.
    2. Select `Record Entire Screen` option if you want to record the video and actions.
- Once the camera icon is visible, click on the screen to take the snapshot / start the recording.
- If you are recording the then click on the 'Stop' icon on menu bar to stop the video recording.
- The video will be saved on the desktop. Meanwhile, if you have captured a snapshot of the screen then the prompt will come up and let you decide the format and the destination to save the image you've captured.

## Opening a file in TextEdit / any other application of our choice from Terminal

```bash
open -a TextEdit 'filename'
```

The -a flag specifies any application you want, so it's applicable to any number of situations, including ones where TextEdit isn't the default editor. Other relevant options:

- -t  opens in the default editor (i.e. if you use BBEdit, TextMate, etc.)
- -e will open the file specifically in TextEdit

## Resolve ChromeDriver opening failure in Mac

Click on the `Apple` menu -> `System Preferences` -> `System and Security` -> `General` -> Message will be shown as 'ChromeDriver is blocked' -> Click on `Allow Anyway`.

## Change Github username and password which are being used from terminal

Recently the Github team has announced that for better protection and privacy users should not use their profile password to push or pull code changes from Github repositories instead they should start using Personal Access Tokens provided by Github. The following process will guide you how to replace your old password with new Personal Access Token generated from your own Github account.

- Check whether credential helper is set or not.  
`> git config --list`  
`credential.helper = osxkeychain`

- Update the credentials via Keychain Access.  
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

## Mobile Testing with Appium in Mac

### Tools required

- JDK
- Maven
- Android Studio
- XCode
- Node.js
- Appium Desktop
- Appium - Command Line Tool present in NPM (Optional)
- Appium Doctor - Command Line Tool present in NPM  (Optional)
- IntelliJ / Eclipse

### Command to install Appium - Command Line Tool in Mac

```bash
sudo npm install -g appium --unsafe-perm=true --allow-root
```

### Fix for uiautomatorviewer2 in Mac

- Search in Google 'Eclipse Project Downloads' or directly visit <https://download.eclipse.org/eclipse/downloads/>

- Choose a 'Build Name' which has support for the Java version you have currently installed on your system.

- Download the 'SWT Binary and Source' for 'Mac OSX (64 bit version)'

  - Java 11 supported SWT: <https://download.eclipse.org/eclipse/downloads/drops4/R-4.21-202109060500/>
  - Java 8 supported SWT: <https://archive.eclipse.org/eclipse/downloads/drops4/R-4.16-202006040540/>
  - Site which has all different archive releases: <https://archive.eclipse.org/eclipse/downloads/>  

- Extract the file you have downloaded (e.g. 'swt-4.21-cocoa-macosx-x86_64.zip'), open the extracted directory and rename 'swt.jar' to 'swt2.jar'.

- Copy and paste the 'swt2.jar' in '/Users/ins667/Library/Android/sdk/tools/lib/x86' and in '/Users/ins667/Library/Android/sdk/tools/lib/x86_64'

- Launch 'uiautomatorviewer2' to verify whether it's running without any issues.

### Practice apps download

- [Android_ApiDemos-debug.apk - Official](https://appium.io/docs/en/about-appium/getting-started/index.html#running-your-first-test)
- [Android_ApiDemos-debug.apk - GitHub](https://github.com/appium/appium/tree/master/sample-code/apps)

### Important Commands

- `adb devices` : Get the UDID of the devices connected.
- `adb shell dumpsys window | grep -E 'CurrentFocus|FocusedApp'` : Get the appPackage and appActivity of an app.

## Setting up Visual Studio Code

### Necessary extensions

- Auto Close Tag
- Auto Import
- Auto Rename Tag
- Babel JavaScript
- Bracket Pair Colorizer
- C/C++
- C/C++ Compile Run
- Code Runner
- Code Spell Checker
- Color Highlight
- CSS Peek
- Debugger for Java
- EditorConfig for VS Code
- ESLint
- Excel Viewer
- Extension Pack for Java
- GitLens - Git supercharged
- Jupyter
- Language Support for Java(TM) by Red Hat
- Live Sass Compiler
- Live Server
- Markdown Preview Github Styling
- markdownlint
- Maven for Java
- Monokai Pro
- Paste and Indent
- Path Intellisense
- PHP Debug
- PHP Extension Pack
- PHP Intelephense
- PHP IntelliSense
- Prettier - Code formatter
- Project Manager for Java
- Pylance
- Python
- Sass
- Test Runner for Java
- Thunder Client
- TSLint
- Visual Studio IntelliCode
- vscode-pdf
- XCode

### Configuration for settings.json

Click on the `Manage` (Screw) icon -> `Settings` (Shortcut: `Command + ,`) -> From the top right corner click on `Open Settings (JSON)`.

```json
{   
    "c-cpp-compile-run.c-flags": "-Wall -Wextra -O0 -std=c18",
    "c-cpp-compile-run.cpp-flags": "-Wall -Wextra -O0 -std=c++20",
    "code-runner.clearPreviousOutput": true,
    "code-runner.executorMap": {
        "typescript": "tsc"
    },
    "code-runner.ignoreSelection": true,
    "code-runner.runInTerminal": true,
    "code-runner.saveFileBeforeRun": true,
    "code-runner.showExecutionMessage": true,
    "color-highlight.markerType": "dot-after",
    "cSpell.ignoreWords": [
        "deepjyoti"
    ],
    "diffEditor.ignoreTrimWhitespace": false,
    "editor.fontSize": 11,
    "editor.suggestSelection": "first",
    "editor.wordWrap": "on",
    "explorer.compactFolders": false,
    "explorer.confirmDelete": false,
    "explorer.confirmDragAndDrop": false,
    "files.autoSaveDelay": 5000,
    "java.configuration.checkProjectSettingsExclusions": false,
    "java.errors.incompleteClasspath.severity": "ignore",
    "java.home": "/Library/Java/JavaVirtualMachines/jdk-11.0.11.jdk/Contents/Home/",
    "java.configuration.runtimes": [
        {
          "name": "JavaSE-1.8",
          "path": "/Library/Java/JavaVirtualMachines/jdk1.8.0_291.jdk/Contents/Home/"
        },
        {
            "name": "JavaSE-11",
            "path": "/Library/Java/JavaVirtualMachines/jdk-11.0.11.jdk/Contents/Home/",
            "sources" : "/Library/Java/JavaVirtualMachines/jdk-11.0.11.jdk/Contents/Home/lib/src.zip",
            "javadoc" : "https://docs.oracle.com/en/java/javase/11/docs/api",
            "default":  true
           }
    ],
    "prettier.singleQuote": false,
    "prettier.tabWidth": 4,
    "python.languageServer": "Default",
    "python.pythonPath": "/Library/Developer/CommandLineTools/usr/bin/python3",
    "terminal.integrated.fontFamily": "Monaco",
    "terminal.integrated.fontSize": 11,
    "workbench.colorTheme": "Monokai Pro (Filter Spectrum)",
    "workbench.iconTheme": "Monokai Pro (Filter Spectrum) Icons",
    "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
    "workbench.editorAssociations": {
        "*.ipynb": "jupyter.notebook.ipynb"
    },
}
```

## Setting up IntelliJ IDEA

### Configuring Appearance

Open up 'IntelliJ IDEA' -> Click on `IntelliJ IDEA` on the menu bar -> `Preferences` -> `Appearance`

- `Theme`: `One Dark Vivid Italic`
- Check `Use custom font`
- `Use custom font`: `.SF NS Text`
- `Size`: `11`

### Configuring Editor

Open up 'IntelliJ IDEA' -> Click on `IntelliJ IDEA` on the menu bar -> `Preferences` -> `Editor` -> `Font`

- `Font`: `Monospaced`
- `Size`: `10`
- `Line height`: `1.1`

### Necessary plugins

Open up 'IntelliJ IDEA' -> Click on `IntelliJ IDEA` on the menu bar -> `Preferences` -> `Plugins`

- Create TestNG XML
- Cucumber for Java
- ExcelReader
- Gherkin
- One Dark theme
- SonarLint

### Changing Java SDK in a project

Open up 'IntelliJ IDEA' -> Click on `File` on the menu bar -> `Project Structure` -> `Project`

- `Project SDK`: Click on the dropdown and select any `Detected SDKs`. If the SDK of your choice is not available then select the `+ Add SDK` option and choose any option feasible to you. You may either go for `Download JDK` option or Click on `JDK` and locate a JDK from your local system.

## Setting up Sublime Text

### Installing Package Control

- Open the command palette by pressing `Command + Shift + P`.
- Type 'Install Package Control', press `Enter`
- After successful installation click on the `OK` button.

__Tip__: For manual installation of the plugin visit: <https://packagecontrol.io/installation>

### Configuration for Preferences.sublime-settings.json

Open up 'Sublime Text' -> Click on `Sublime Text` on the menu bar -> `Preferences` -> `Settings` (Shortcut: `Command + ,`)

```json
{
    "ignored_packages":
    [
        "Vintage",
    ],
    "color_scheme": "Packages/ayu/ayu-dark.sublime-color-scheme",
    "theme": "ayu-dark.sublime-theme",
    "font_size": 11,
}
```

### Necessary packages

- A File Icon
- All Autocomplete
- AutoFileName
- ayu
- BracketHighlighter
- Emmet
- Package Control
- SideBarEnhancements
- SublimeLinter
- [SublimeLinter](https://packagecontrol.io/search/SublimeLinter)
- [SublimeLinter-javac](https://packagecontrol.io/packages/SublimeLinter-javac)
- [SublimeLinter-jshint](https://packagecontrol.io/packages/SublimeLinter-jshint)
- [Sublime​Linter-tslint](https://packagecontrol.io/packages/SublimeLinter-tslint)
- [Sublime​Linter-pylint](https://packagecontrol.io/packages/SublimeLinter-pylint)
- [SublimeLinter-php](https://packagecontrol.io/packages/SublimeLinter-php)
- [Sublime​Linter-ruby](https://packagecontrol.io/packages/SublimeLinter-ruby)
- [SublimeLinter-clang](https://packagecontrol.io/packages/SublimeLinter-clang)
- [SublimeLinter-cpplint](https://packagecontrol.io/packages/SublimeLinter-cpplint)
- [Sublime​Linter-html-tidy](https://packagecontrol.io/packages/SublimeLinter-html-tidy)
- [Sublime​Linter-csslint](https://packagecontrol.io/packages/SublimeLinter-csslint)
- [SublimeLinter-json](https://packagecontrol.io/packages/SublimeLinter-json)
- [SublimeLinter-shellcheck](https://packagecontrol.io/packages/SublimeLinter-shellcheck)
- SublimeREPL
- Terminal
- Terminus
- zzz A File Icon zzz

### Custom build systems

Command to open the directory where all the user defined build systems are saved:
`cd "~/Library/Application\ Support/Sublime\ Text/Packages/User" && open .`

python3-runner-repl.sublime-build:

```json
{
    "target": "run_existing_window_command", 
    "id": "repl_python_run",
    "selector": "source.python",
    "file": "config/Python/Main.sublime-menu"
}
```

python3-runner-terminal.sublime-build:

```json
{
    "shell_cmd": "osascript -e 'tell app \"Terminal\" to do script \"cd $file_path && python3 -u $file\"'",
    "working_dir": "$file_path",
    "selector": "source.python",
    "env": {"PYTHONIOENCODING": "utf-8"}
}
```

python3-runner-terminus.sublime-build:

```json
{
    "target": "terminus_exec",
    "cancel": "terminus_cancel_build",
    "cmd": [
        "python3", "-u", "$file"
    ],
    "working_dir": "$file_path",
    "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
}
```

javac-compile-run-terminus.sublime-build:

```json
{
    "target": "terminus_exec",
    "cancel": "terminus_cancel_build",
    "shell_cmd": "javac $file && java $file_base_name",
    "working_dir": "$file_path"
}
```

## Setting up Charles

### Register Charles

- Open up 'Charles' -> `Help` -> `Register Charles`
- Enter `Username` and `Password`.
- Click on `OK`.
- Restart 'Charles'.

### Installing Charles Root Certificate on your Mac

- Open up 'Charles' -> `Help` -> `SSL Proxying` -> `Install Charles Root Certificate`
- Following the above step will open up 'Keychain Access'.
- Search for 'Charles' in the search bar.
- Once you are able to find the certificate after the search -> Double click on the certificate -> Click on the arrow mark next to `Trust` and change the details from the dropdown as listed down below,  
`When using this certificate`: `Always Trust`
- You will be asked to enter your computer / admin password -> `Update settings`
- Once the changes are done close the window.

### Installing Charles Root Certificate on your Mobile

- Before installing 'Charles Root Certificate' on your mobile make sure that your laptop and your mobile is connected to the same WiFi network and proxying settings are setup correctly. To configure the proxying settings follow the given steps:
  - While 'Charles' is open go to `Help` -> `Local IP Address` -> Get the `IP Address` for `Network Interface`: `en0` -> Close the window
  - Go to `Proxy` -> `Proxy Settings` -> Get the `HTTP Proxy` port number
  - Open up your mobile -> Settings -> WiFi -> Click on the `>` icon or long press on the network you are connected to -> `Manage network settings` -> `Show advanced options`
  - Now change `Proxy`: `Manual`
  - Under `Proxy host name` enter the internal IP address of your computer that you have noted down earlier.
  - Under `Proxy port` enter the HTTP proxy port number that you have noted down earlier.
  - Save the changes.
  - Once you come back to Charles you will find a popup, click on the 'Allow' button of that popup.
- Now open up any browser on your mobile and enter <http://chls.pro/ssl>.
- Download the 'SSL certificate' and click on it to start the installation.
- While installing it may ask you to setup a PIN.
- Fill up the details as given below,  
`Certificate Name`: `Charles Root Certificate`  
`Used for`: `VPN and apps`
- Click on `OK` button.

### Enable and configure SSL Proxying Settings

- Open up 'Charles' -> `Proxy` -> `SSL Proxying Settings`
- Click on `Enable SSL Proxying`.
- Click on the `Add` button which is present under the `Include` section.
- In the `Host` field
  - If you want to monitor all the traffic then type `*`.
  - If you want to monitor only a specific set of traffic related to your host then enter `*hostname.extension` (i.e. `*makemytrip.com`).
- In the `Port` field you may either enter `*` or enter `443`, anything of your choice.
- Click on `OK` -> `OK`

## Shortcuts

- `Command + Space` : Open up 'Spotlight Search' for searching any application, document etc. on your system or on the web.
- `Command + Q` : Quit the currently open application.
- `Command + M` : Minimize the focused window.
- `Command + Shift + 3` : Capture a full size screenshot of the window.
- `Command + Shift + 4` : Capture a portion of the screen.
- `Command + Tab` : Switch between applications.
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
- `Mouse1_Double_Click` (on any text): __(iTerm2)__ Select / highlight the text in iTerm2 and copy it to clipboard.
- `Mouse3_Click` : __(iTerm2)__ Paste the content from the clipboard in iTerm2.

## Commands

- `sudo shutdown -h now` : Shuts down your system immediately.
- `sudo shutdown -r now` : Restarts your system immediately.
- `open .` : Open the current directory in Finder.
- `ls > ~/Desktop/files.txt` : __(I/O Redirection)__ Redirects the output of 'ls' command to 'files.txt', overwrites the existing content if the file already exists.
- `ls >> ~/Desktop/files.txt` : __(I/O Redirection)__ Redirects the output of 'ls' command to 'files.txt', appends to the existing content if the file already exists.
- `ls | open -fe` : __(I/O Redirection)__ Redirects the output of 'ls' command and opens it in default text editor of the system (i.e. TextEdit).
- `ls | pbcopy` : __(I/O Redirection)__ Redirects the output of 'ls' command to the clipboard.
