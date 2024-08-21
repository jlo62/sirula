Hi, this is a fork of [sirula](https://github.com/DorianRudolph/sirula) that includes extra PRs that are pending for the main repo.\
This fork is available as [sirula-extended-git on the AUR](https://aur.archlinux.org/packages/sirula-extended-git)

If you encounter a issue with sirula, open a Issue over there.\
If you want to have a pending merge request implemented here, please open a issue here.

This fork currently includes these additional config options:
* launch the apps in cgroups
* close the window on unfocus
* add a newline between description and title
* drop old history items
* set the namespace to sirula for window rules
* add keypad navigation keys

# Sirula

Sirula (simple rust launcher) is an app launcher for wayland.
Currently, the only feature is launching apps from `.desktop` files.
Feel free to submit pull requests for any feature you like.

I wrote sirula partially to learn rust, so do not expect perfect rust code.
I'd be happy to hear any criticism of my code.

## Examples

`sample-config/a`:

![](sample-config/a/sirula.gif)
[open](https://raw.githubusercontent.com/jlo62/sirula/master/sample-config/sirula.gif)

`sample-config/b`: Overlay in the center of the screen.

![](sample-config/b/sirula.png)
## Building

- Dependency: [gtk-layer-shell](https://github.com/wmww/gtk-layer-shell)
- Build: `cargo build --release`
  - Optionally, `strip` the binary to reduce size
- Alternatively, install with `cargo install --path .`
- There is also an unofficial [AUR package](https://aur.archlinux.org/packages/sirula-git/)

## Configuration

Use `config.toml` and `style.css` in your `.config/sirula` directory.
See `sample-config` for documentation.
