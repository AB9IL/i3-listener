# i3-listener
i3wm interprocess communication (ipc) listener with functions for managing floating windows and a master-stack layout.

### Usage:
Call this script from the i3 config file or from something like .profile, which runs on login.  It requires two arguments: floating window width and height as a percentage of screen size.

<code>
exec --no-startup-id exec i3-listener 75 85
</code>

### Required Python packages:
pyautogui
i3ipc
sys

### Acknowledgements:
This script was inspired by things I learned from...  
[Budrich's i3 floating mode listener](https://github.com/budRich/i3ipc-python/blob/master/examples/floating-mode.py)  
[Aduros's i3 two column layout](https://github.com/aduros/dotfiles/blob/master/home/.config/i3/column-layout)  
