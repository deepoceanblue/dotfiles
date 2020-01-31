# dotfiles

Configs for linux cli apps.

For details read comments inside each config file. 

## tmux

Load with: `tmux -f .tmux.conf` at a startup, or `:source .tmux.conf` at a run-time from tmux command prompt.

Some *alternative* commodity bindings but without overhauling the default keymap.
tmux is industry standard and vanilla setups are everywhere.

## xmodmap configuration

Load with: `xmodmap keys_{mods,pl}` from your `.xinitrc` or to reload from within the X session.

### xmodmap/keys_mods

  - `Mode_switch` replaces `CapsLock` 
  - force proper binding (keycode and keysym) for: Alt_L (AltGr), BackSpace, Super_L.

### xmodmap/keys_pl

  - Polish keyboard layout with additional keysyms accessible with `Mode_switch` (bound to `CapsLock`).
  - `Mode_switch`-hjkl defined as arrow keys, to enable zero-conf vim-like navigation in most applications.
