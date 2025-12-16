# Productivity Mouse Configuration

The configuration in this repository was designed for the [UtechSmart Wireless VenusPro Gaming Mouse](https://www.utechsmart.com/products/DS-2833.html) ([Amazon](https://www.amazon.com/UtechSmart-transmission-technology-Ergonomic-programmable/dp/B07XP4K152)). Some attractive qualities include:

- Relatively affordable, making it feasible for multiple setups and easy to replace
- Reliable (unlike Logitech G600, which is prone to double-clicking)
- Responsive wireless with good battery life, and can be rechared while being used in wired mode
- On-board memory (key bindings persist without locally installed software)

Obviously, the choices were made according to my personal preference. For example, one could argue that the "close tab" button conceptually belongs at button 11, but I am accustomed to having it on 8. You are encouraged to make it your own and customize the configuration to your desired specifications.


## Windows installation instructions

The mouse must be first configured on a Windows device. If desired, the 4t Tray Minimizer software must be installed on all applicable Windows devices.

1. Install provided UtechSmart software and import [utechsmart-venuspro-settings.jmk](/utechsmart-venuspro-settings.jmk)

2. Install [4t Tray Minimizer Free](https://www.4t-niagara.com/tray.html) and import [4t-settings.4t-min_ini](/4t-settings.4t-min_ini)

    4t Tray Minimizer is a lightweight tool for conveniently minimizing and restoring windows from the tray. I have found it convenient across over a decade of use, but it is not required.

The 12 programmable buttons on the side panel are accessible to the thumb as 4 rows of 3 columns and are bound as follows, acting on the active window:

| Button | Shortcut | Description |
|--------|----------|-------------|
| 1 | `Shift + Win + Left` | Move to monitor on left |
| 2 | `Win + Up` | Fullscreen |
| 3 | `Shift + Win + Right` | Move to monitor on right |
| 4 | `Ctrl + Win + W` | Minimize to tray (4t) |
| 5 | `Win + Tab` | [Task View](https://support.microsoft.com/en-us/windows/how-to-multitask-in-windows-b4fa0333-98f8-ef43-e25c-06d4fb1d6960) |
| 6 | `Ctrl + Win + U` | Open menu to restore from tray (4t) |
| 7 | `Ctrl + Win + Left` | Switch to left desktop |
| 8 | `Ctrl + W` | Close tab |
| 9 | `Ctrl + Win + Right` | Switch to right desktop |
| 10 | `Ctrl + Shift + Tab` | Previous tab |
| 11 | `Ctrl + Shift + W` | Close window |
| 12 | `Ctrl + Tab` | Next tab |


## macOS installation instructions

The following instructions extend the configuration to seamlessly operate on and switch between both Windows and macOS devices. All desired features must be installed on all applicable devices.

1. Install [Karabiner Elements](https://karabiner-elements.pqrs.org/) and clone this repository into `~/.config/karabiner`:

    ```
    git clone git@github.com:jirehhuang/productivity-mouse-config.git ~/.config/karabiner
    ```

2. Install [Rectangle](https://rectangleapp.com/) and import [RectangleConfig.json](/RectangleConfig.json)

3. Install [Scroll Reverser](https://pilotmoon.com/scrollreverser/) and select only the following:
    - Enable Scroll Reverser
    - Reverse Vertical
    - Reverse Mouse
    - Start at login

The programmable buttons are reconfigured to accomplish the following:

| Button | Mouse Shortcut | Karabiner Mapping | Description |
|--------|----------------|-------------------|-------------|
| 1 | `Shift + Cmd + Left` | `Ctrl + Option + Cmd + Left` | Move to monitor on left (Rectangle) |
| 2 | `Cmd + Up` | `Ctrl + Cmd + F` | Fullscreen |
| 3 | `Shift + Cmd + Right` | `Ctrl + Option + Cmd + Right` | Move to monitor on right (Rectangle) |
| 4 | `Ctrl + Cmd + W` | `Cmd + M` | Minimize window |
| 5 | `Cmd + Tab` | `Ctrl + Up` | Mission Control |
| 6 | `Ctrl + Cmd + U` | `Ctrl + Down` | App Exposé |
| 7 | `Ctrl + Cmd + Left` | `Ctrl + Left` | Switch to left desktop |
| 8 | `Ctrl + W` | `Cmd + W` | Close tab |
| 9 | `Ctrl + Cmd + Right` | `Ctrl + Right` | Switch to right desktop |
| 10 | `Ctrl + Shift + Tab` | N/A | Previous tab |
| 11 | `Ctrl + Shift + W` | `Cmd + Shift + W` | Close window |
| 12 | `Ctrl + Tab` | N/A | Next tab |
