# tuios

My [tuios](https://github.com/Gaurav-Gosain/tuios) config, cloned into
`~/.config/tuios`:

```bash
git clone https://github.com/lararosekelley/tuios ~/.config/tuios
```

- `config.toml`: keybindings, the status bar, and the callie theme in `themes/`.
- `status-cells/`: the scripts behind the status bar cells.
- `default-session/`: the default session layout. `layout.json` lists the
  workspaces and their panes, `layout.py` decides which ones a session gets, and
  `session.py` builds them in tuios.
- `bin/tui`: opens a session per repo listed in `repos`, plus a home session on
  `~`, and attaches. Put `bin` on `PATH` and load its completions with
  `tui completions bash` or `tui completions fish`.

## Tests

```bash
python3 -m unittest discover -s tests
```
