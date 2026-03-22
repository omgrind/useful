# useful

## Anki Cards

```plaintext
пожалуйста, создай 50 anki карточек по теме,
если что-то не учтено в pdf, дополни,
обязательно перепроверь всю информацию,
опирайся на официальные и уважаемые источники
в качестве разделителя используй |
выдай их в формате кода
```

## Bash commands

**Duplicate one file into several:**

```bash
tee < source.file destination{0..9}.file > /dev/null
```

**List files in lines count sort by extension:**

```bash
find . -type f -name '*.md' | xargs wc -l | sort -n
```

**List files in update time order:**

```bash
ls -larth
```

**Remove all\* docker containers:**

```bash
docker container ls -aq | awk '{print $1}' | xargs docker container rm
```

**Remove all\* docker images:**

```bash
docker images -q | awk '{print $1}' | xargs docker image rm
```

**Remove all\* docker volumes:**

```bash
docker volume ls -q | xargs docker volume rm
```

## Tmux Cheat Sheet

### Prefix Key

`Ctrl+b` - default prefix (press before commands)

### Sessions

- `tmux new -s name` - create new session
- `tmux ls` - list sessions
- `tmux a -t name` - attach to session
- `Ctrl+b d` - detach from session

### Windows

- `Ctrl+b c` - create window
- `Ctrl+b n` - next window
- `Ctrl+b p` - previous window
- `Ctrl+b w` - list windows
- `Ctrl+b ,` - rename window
- `Ctrl+b &` - kill window

### Panes

- `Ctrl+b %` - split vertical
- `Ctrl+b "` - split horizontal
- `Ctrl+b arrow` - navigate panes
- `Ctrl+b x` - kill pane
- `Ctrl+b z` - toggle zoom

### Scroll

- `Ctrl+b [` - enter scroll mode
  - `arrow` - navigate
  - `q` - exit scroll mode
