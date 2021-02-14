<h1 id='table-of-contents'>TABLE OF CONTENTS</h1>

- [VIM](#vim)
  - [Commands](#commands)
    - [Insert](#insert)
    - [Exit / Save](#exit--save)
    - [Move](#move)
    - [Copy](#copy)
    - [Delete](#delete)
    - [Paste](#paste)
    - [Replace](#replace)
    - [Undo](#undo)
    - [Redo](#redo)
    - [Search](#search)
    - [Execute Shell Commands](#execute-shell-commands)
    - [Recording](#recording)
    - [Select Text and Save as New File](#select-text-and-save-as-new-file)
    - [Insert Content](#insert-content)
    - [Change Window Focus](#change-window-focus)
    - [Help](#help)

# VIM

```Bash
  vimtutor
```

## Commands

[Go Back to Contents](#table-of-contents)

### Insert

```Bash
  a           # Append text after the cursor
  A           # End of line in insert mode
  i           # Insert mode
  o           # Creates a new line below the cursor and place you in Insert mode
  O           # Creates a new line above the cursor and place you in Insert mode
  R           # Insert mode (like Insert key)
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
  $           # End of the line
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

### Copy

```Bash
  v           # Visual model
      y /      # Copy selected text
      p       # Paste selected text
  yw          # Copy single word
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
  # Option ---------------------------------------
    :set ic         # Search word, ignore case sensitive
    :set noic       # Disable case sensitive
    :set hls        # Activate highlight
    :set nohlsearch # Deactivate highlight
    /ign:ore\c       # Ignore case for just one search
  # Option ---------------------------------------
  ?           # Search backwards
  option n    # Next
  option N    # Previous
```

### Execute Shell Commands

```Bash
  :!          # External commands
```

### Recording

```Bash
  q           # Stop recording
```

### Select Text and Save as New File

```Bash
  v           # --Visual-- mode
              # Select your text (using h, j, k, l)
              # :w to save (:'<,'>w)
```

### Insert Content

```Bash
  :r path/file   # Will copy the content of the file as paste under your cursor
  :r !ls Desktop # Will paste all the filenames under your cursor
```

### Change Window Focus

```Bash
  Ctrl+w        # Switch window focus
```

### Help

```Bash
  :help
  :help w
  :help c_CTRL-D
  :help insert-index
  :help user-manual
```
