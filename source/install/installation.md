### Installation

- **macOS**: Double click to open `EthereumStudio-x.x.x.dmg` and drag `Ethereum Studio` to the application folder.
    - In case of system prompts *"“Ethereum Studio” can’t be opened because Apple cannot check it for malicious software."*, Open *System Perference*, Go to *Security and Privacy*, Click *Open Anyway* in *General* section to allow Ethereum Studio to run.
- **Windows**: Double click to run the `EthereumStudio-x.x.x.exe`.
    - If there is a warning afters run the exe file, please click “continue” on the warning page.
- **Linux**: Double-click to open `EthereumStudio-x.x.x.AppImage`.
    - If application doesn't respond,double click to select *Properties* => *Permissions* => *Execute*, and tick the *Allow executing file as program* option. Close the properties window and double-click to open the application (different Linux distributions may have different installation methods).
    - **After Installation on Linux:** Ethereum Studio uses `inotify` by default on Linux to monitor directories for changes. Users will need to increase the amount of inotify watchers to ensure the file tree is refreshed properly.
        - To increase inotify watchers at boot, execute the following command in Terminal: `echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p`