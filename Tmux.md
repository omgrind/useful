# Tmux

## Prefix Key

`Ctrl+b` - default prefix (press before commands)

## Sessions

- `tmux new -s name` - create new session
- `tmux ls` - list sessions
- `tmux a -t name` - attach to session
- `Ctrl+b d` - detach from session

## Windows

- `Ctrl+b c` - create window
- `Ctrl+b n` - next window
- `Ctrl+b p` - previous window
- `Ctrl+b w` - list windows
- `Ctrl+b ,` - rename window
- `Ctrl+b &` - kill window

## Panes

- `Ctrl+b %` - split vertical
- `Ctrl+b "` - split horizontal
- `Ctrl+b arrow` - navigate panes
- `Ctrl+b x` - kill pane
- `Ctrl+b z` - toggle zoom

## Scroll

- `Ctrl+b [` - enter scroll mode
  - `arrow` - navigate
  - `q` - exit scroll mode
