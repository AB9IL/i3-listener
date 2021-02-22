# i3-listener
i3wm interprocess communication (ipc) listener with functions for managing floating windows and a master-stack layout.

### Usage:
Call this script from the i3 config file or from something like .profile, which runs on login.  It requires two arguments: floating window width and height as a percentage of screen size.  Other code _could_ be incorporated into the script to make certain applications always float, for example terminals or a web browser.  Plan to use a separate listener for things which need to be called only when needed, such as a "window swallowing" or "promote-window" script.

<code>
exec --no-startup-id exec i3-listener 75 85
</code>

### Required Python packages:
pyautogui
i3ipc
sys

### Acknowledgements:
This script was inspired by things I learned from...  
[Budrich: i3 floating mode listener](https://github.com/budRich/i3ipc-python/blob/master/examples/floating-mode.py)  
[Aduros: i3 two column layout](https://github.com/aduros/dotfiles/blob/master/home/.config/i3/column-layout)  
[Aduros: i3 promote window](https://github.com/aduros/dotfiles/blob/master/home/.config/i3/promote-window)  
