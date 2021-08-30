# tmux-autoreload [![version](https://img.shields.io/github/v/tag/b0o/tmux-autoreload?style=flat&color=yellow&label=version&sort=semver)](https://github.com/b0o/tmux-autoreload/releases) [![license: MIT](https://img.shields.io/github/license/b0o/tmux-autoreload?style=flat&color=green)](https://mit-license.org)

tmux-autoreload watches your tmux configuration file and automatically reloads
it on change.

## Install

```sh
### With Tmux Plugin Manager (https://github.com/tmux-plugins/tpm)
# Add the following line to your tmux.conf:
set-option -g @plugin 'b0o/tmux-autoreload'

### Or Manually Install
# Clone the repo to your desired location
$ git clone https://github.com/b0o/tmux-autoreload /path/to/tmux-autoreload
# Add the following line to your tmux.conf:
run-shell "/path/to/tmux-autoreload/tmux-autoreload.tmux"
```

## Usage

That's it! When you edit and write your `tmux.conf`, tmux-autoreload will
tell tmux to source it.

### Advanced Usage

<!-- USAGE -->

```

Usage: tmux-autoreload.tmux [-f] [OPT...]

Watches your tmux configuration file and automatically reloads it on change.

Options
  -h      Display usage information.
  -v      Display tmux-autoreload version and copyright information.
  -f      Run in foreground (do not fork).
  -k      Kill the running instance of tmux-autoreload.
  -s      Show status of tmux-autoreload.
  -m MSG  Display MSG on all clients.
  -M MSG  Display MSG on all clients (wait for keypress).

To enable tmux-autoreload, install TPM (https://github.com/tmux-plugins/tpm) and add the
following line to the end of your tmux configuration file:

    set-option -g @plugin 'b0o/tmux-autoreload'

If you do not use a plugin manager, you can run tmux-autoreload directly:

    run-shell "/home/maddy/proj/tmux-autoreload/tmux-autoreload.tmux"

```

<!-- /USAGE -->

## License

<!-- LICENSE -->

&copy; 2021 Maddison Hellstrom

Released under the MIT License.

<!-- /LICENSE -->
