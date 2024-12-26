# tinted-ghostty

A Tinted Theming template for [Ghostty] with [Base16] themes

### Themes

Copy all the files in `themes/` into any of these directories:

1. `$XDG_CONFIG_HOME/ghostty/themes`
2. `$PREFIX/share/ghostty/themes`

Ghostty recognizes files in these directories as themes that can be selected e.g.

```
theme = base16-3024
```

### Using with Tinty

For usage with [Tinty]:

1. Add the following to your Ghostty config `~/.config/ghostty/config`:

```
theme = ~/.local/share/share/tinted-theming/tinty/tinted-ghostty-themes-file
```

2. Add the following to `~/.config/tinted-theming/tinty/config.toml`:

   ```toml
   [[items]]
   path = "https://github.com/bezhermoso/tinted-ghostty"
   name = "tinted-ghostty"
   themes-dir = "themes"
   supported-systems = ["base16"]
   ```

3. `tinty apply ...` to apply the theme you like.

4. Trigger `reload_config` in Ghostty. The default keybinding for this are `Ctrl + Shift + ,` (`Cmd + Shift + ,` for
   macOS)

[Ghostty]: https://ghostty.org
[Base16]: https://github.com/tinted-theming/home/blob/main/styling.md
[Tinty]: https://github.com/tinted-theming/tinty
