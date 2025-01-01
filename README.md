# ALWO (App Launcher and Worspace Organizer)
ALWO is an app launcher which launches multiple apps at the same time as required by the user's workflow.

Checkout [ALWO for Windows](https://github.com/kaushik-kalesh/alwo)

### Features:
- Launch mutliple apps at the same time
- Open apps in different virtual desktops 
- Have multiple workflows 

## Installation
1. Download the binaries from the [releases page](https://github.com/kaushik-kalesh/alwo-linux/releases)
2. Make the `alwo` binary executable and move it to your local scripts directory (to access it from anywhere by your user) or to `/bin` for system wide access
3. Refer [usage](#usage)

## Usage
1. Make a config file, default location is `~/.config/alwo/config`
2. Provide a workspace name followed by `;` 
3. Add the list of applications assoicated with the workspace along segregated by their desktops. Desktops are numbered from 0 followed by `:`
Example:
```txt
work;
0:
chromium --incognito
1:
code [5]
kitty
2:
discord

write;
0:
lowriter
1:
spotify
```
5. To start the `work` workspace, run the following command
```bash
alwo work
``` 
6. Run `alwo -h` for more information