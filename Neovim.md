# Neovim

## Modes

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

## Explorer

### Opening

- `:Ex` or `:Explore` – Open file explorer  
- `:Sex` – Horizontal split  
- `:Vex` – Vertical split  

### Navigation

- `Enter` – Open file/directory  
- `-` – Go up one level  
- `o` – Open in a new window  
- `v` – Open in vertical split  
- `s` – Open in horizontal split  

### Operations

- `%` – Create file  
- `d` – Create directory  
- `D` – Delete  
- `R` – Rename  

## File Operations

- `:w` – Save  
- `:q` – Quit  
- `:wq` – Save and quit  
- `:q!` – Quit without saving  
- `:e filename` – Open file  
- `:enew` – New buffer  

## Selection (Visual mode)

- `v` – Character-wise selection  
- `V` – Line-wise selection  
- `Ctrl + v` – Block selection  

## Copy, Paste, Delete

### Copy (yank)

- `y` – Copy selection  
- `yy` – Copy line  
- `y$` – Copy to end of line  

### Paste

- `p` – Paste after  
- `P` – Paste before  

### Delete / Cut

- `d` – Delete selection  
- `dd` – Delete line  
- `d$` – Delete to end of line  
- `x` – Delete character  

## Editing

- `u` – Undo  
- `Ctrl + r` – Redo  
- `.` – Repeat last action  
- `r` – Replace character  
- `~` – Toggle case  

## Search

- `/text` – Search forward  
- `?text` – Search backward  
- `n` – Next result  
- `N` – Previous result  

## Navigation

- `w` – Move forward by words  
- `b` – Move backward by words  
- `0` – Start of line  
- `$` – End of line  
- `gg` – Start of file  
- `G` – End of file  

## Windows (splits)

- `:split` – Horizontal split  
- `:vsplit` – Vertical split  

### Switching

- `Ctrl + w + h` – Move left  
- `Ctrl + w + j` – Move down  
- `Ctrl + w + k` – Move up  
- `Ctrl + w + l` – Move right
