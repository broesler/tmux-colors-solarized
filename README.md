# Solarized Color Theme tmux Configuration

A [tmux](https://github.com/tmux/tmux) solarized theme using Ethan Schoonover’s [Solarized color scheme](http://ethanschoonover.com/solarized). This fork has been updated to work with `tmux` version `2.9a`.

## Repositories
  * This theme as a single repository: [/broesler/tmux-colors-solarized](https://github.com/broesler/tmux-colors-solarized)
  * The main solarized repository: [/altercation/solarized](https://github.com/altercation/solarized)

## Installation
Clone the repository:

    mkdir -p ~/.tmux/plugins
    git clone  https://github.com/broesler/tmux-colors-solarized ~/.tmux/plugins/tmux-colors-solarized

These config snippets should be added to your `~/.tmux.conf` configuration file. Four themes are provided so you can pick and choose:

- `256` (default)
- `dark`
- `light`
- `base16`

### Installation as-is
In your `.tmux.conf`, set the theme option, then source the main script:

```tmux
    set -g @colors-solarized 'dark'   # choose '256', 'dark', 'light', 'base16'
    run-shell ~/.tmux/plugins/tmux-colors-solarized/tmuxcolors.tmux
```

### Installation with [Tmux Plugin Manager](https://github.com/tmux-plugins/tpm)

Set the theme option, then add plugin to the list of TPM plugins in `.tmux.conf`:

    set -g @colors-solarized 'dark'   # choose '256', 'dark', 'light', 'base16'
    set -g @plugin 'plugins/tmux-colors-solarized'

Hit `prefix` + <kbd>I</kbd> to fetch the plugin and source it. The plugin should now be working.

This color scheme is tested with tmux >= 2.9a. tmux 1.1 is reported as not working.

## Screenshot
Here is a screenshot of a tmux session captured from a gnome-terminal.

![screenshot](https://github.com/broesler/tmux-colors-solarized/raw/master/tmuxcolors.png)
