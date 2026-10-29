# sway helper scripts

Some scripts to help me work with sway

## Overview

These scripts use (rofi)[https://github.com/davatorium/rofi] to show and run frequently used sway commands and key-sequences in menus.  

Menus can be stored in text files such as the following


sway.menu
```
🪟🇩     apps menu || rofi -show drun -show-icons 
🪟↩️     new terminal 🖥️ || swaymsg exec foot

🪟⬆️🇪   exit Sway || ~/.local/bin/sway/_mymenu ~/.local/bin/sway/exit.menu


fw   find window || ~/.local/bin/sway/_my_choose_window 
bm   goto bookmark || ~/.local/bin/sway/_my_goto_bookmark 
```

and displayed using 
```bash
 _mymenu ~/.local/bin/sway.menu
```


The key sequences shown are for information only - they should match the ones defined in ~/.config/sway/config.   Choosing them from the menu actually runs the command shown after the double pipe symbol. In the case of 'fw' for find window,  the 'kw' is there so that you can enter 'kw' to select the command quickly (in the menu only).



