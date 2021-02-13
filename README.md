<h1 id='table-of-contents'>TABLE OF CONTENTS</h1>

- [VIM](#vim)
  - [Commands](#commands)
    - [Insert](#insert)
    - [Exit / Save](#exit--save)
    - [Move](#move)
    - [Delete](#delete)
    - [Paste](#paste)
    - [Replace](#replace)
    - [Undo](#undo)
    - [Redo](#redo)
    - [Search](#search)
    - [Execute Shell Commands](#execute-shell-commands)
    - [Recording](#recording)

# VIM

## Commands

### Insert

```Bash
  A           # End of line in insert mode
  i           # Insert mode
```

### Exit / Save

```Bash
  :q!         # Exit without saving
  :wq         # Save and exit
  :w filename # Save as
```

### Move

```Bash
  j           # Down
  k           # Up
  h           # Left
  l           # Right
  w           # Beginning of the word
  e           # End of the word
  0           # Beginning of the line
  Ctrl + g    # Show where you are in the file
  Shift + g   # Bottom of the file
  gg          # Top of the file
  number + G  # Go to line
  %           # Find closing brackets
  Ctrl + o    # Takes you back to older positions
  Ctrl + i    # Takes you back to newer positions

  Ctrl + e    # Move down
  Ctrl + y    # Move up
```

### Delete

```Bash
  x           # Delete single character
  dw          # Delete word
  d$          # Delete right until the end
  d2w         # Delete 2 words
```

### Paste

```Bash
  p           # Paste below
```

### Replace

```Bash
  r               # Replace character
  ce              # Replace until the end of the word (e)
  c$              # Replace until the end of the line ($)
  :s/old/new/g    # Substitute globally
  :%s/old/new/g   # Substitute globally in the line
  :%s/old/new/gc  # Substitute globally in the line and prompt y/n
  :#,#s/old/new/g # Substitute first # line, second # number of lines
```

### Undo

```Bash
  u           # Undo
  U           # Undo entire line
```

### Redo

```Bash
  Ctrl + r    # Redo
```

### Search

```Bash
  /           # Search forward
  option n    # Next
  option N    # Previous
  ?           # Search backwards
```

### Execute Shell Commands

```Bash
  :!          # External commands
```

### Recording

```Bash
  q           # Stop recording
```
