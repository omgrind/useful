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

## Tmux

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

## Neovim

### Modes

- `Esc` – Normal mode  
- `i` – Insert mode (before cursor)  
- `a` – Insert mode (after cursor)  
- `I` – Insert at beginning of line  
- `A` – Insert at end of line  
- `o` – New line below + Insert mode  
- `O` – New line above + Insert mode  
- `v` – Visual mode (character-wise)  
- `V` – Visual Line mode (line-wise)  
- `Ctrl + v` – Visual Block mode  
- `R` – Replace mode  

### Explorer

#### Opening

- `:Ex` or `:Explore` – Open file explorer  
- `:Sex` – Horizontal split  
- `:Vex` – Vertical split  

#### Navigation

- `Enter` – Open file/directory  
- `-` – Go up one level  
- `o` – Open in a new window  
- `v` – Open in vertical split  
- `s` – Open in horizontal split  

#### Operations

- `%` – Create file  
- `d` – Create directory  
- `D` – Delete  
- `R` – Rename  

### File Operations

- `:w` – Save  
- `:q` – Quit  
- `:wq` – Save and quit  
- `:q!` – Quit without saving  
- `:e filename` – Open file  
- `:enew` – New buffer  

### Selection (Visual mode)

- `v` – Character-wise selection  
- `V` – Line-wise selection  
- `Ctrl + v` – Block selection  

### Copy, Paste, Delete

#### Copy (yank)

- `y` – Copy selection  
- `yy` – Copy line  
- `y$` – Copy to end of line  

#### Paste

- `p` – Paste after  
- `P` – Paste before  

#### Delete / Cut

- `d` – Delete selection  
- `dd` – Delete line  
- `d$` – Delete to end of line  
- `x` – Delete character  

### Editing

- `u` – Undo  
- `Ctrl + r` – Redo  
- `.` – Repeat last action  
- `r` – Replace character  
- `~` – Toggle case  

### Search

- `/text` – Search forward  
- `?text` – Search backward  
- `n` – Next result  
- `N` – Previous result  

### Navigation

- `w` – Move forward by words  
- `b` – Move backward by words  
- `0` – Start of line  
- `$` – End of line  
- `gg` – Start of file  
- `G` – End of file  

### Windows (splits)

- `:split` – Horizontal split  
- `:vsplit` – Vertical split  

#### Switching

- `Ctrl + w + h` – Move left  
- `Ctrl + w + j` – Move down  
- `Ctrl + w + k` – Move up  
- `Ctrl + w + l` – Move right 
