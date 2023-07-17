ChatGPT Prompt: 
```
Can you make me a nice tmux cheatsheet including creating and renaming sessions and windows and other common use cases? Ideally this cheatsheet would be compact/concise to fit on one page of paper.
```

Absolutely! Here is a compact and concise cheatsheet for `tmux` with commonly used commands, including those for creating and renaming sessions and windows:

**Session Management**
- Create new session: `tmux new-session -s my_session`
- Attach to a session: `tmux attach-session -t my_session`
- List sessions: `tmux list-sessions`
- Detach from a session: `Ctrl+b, d`
- Kill a session: `tmux kill-session -t my_session`
- Rename a session: `Ctrl+b, $` (then type the new name and press Enter)

**Window Management**
- Create a new window: `Ctrl+b, c`
- Go to previous window: `Ctrl+b, p`
- Go to next window: `Ctrl+b, n`
- Go to a specific window number (0-indexed): `Ctrl+b, <window number>`
- List windows: `Ctrl+b, l`
- Kill current window: `Ctrl+b, &` (then confirm with 'y')
- Rename current window: `Ctrl+b, ,` (then type the new name and press Enter)

**Pane Management**
- Split pane horizontally: `Ctrl+b, %`
- Split pane vertically: `Ctrl+b, "`
- Switch to another pane: `Ctrl+b, <arrow key>`
- Kill pane: `Ctrl+b, x` (then confirm with 'y')
- Swap panes: `Ctrl+b, {` (move current pane left), `Ctrl+b, }` (move current pane right)

**Copy Mode and Scrolling**

- Enter copy mode: `Ctrl+b`, `[`
- Exit copy mode: `q`
- Scroll up/down (line by line): `<up/down arrow keys>` in copy mode
- Scroll up/down (page by page): `fn` + `<up/down arrow keys>` in copy mode on a MacBook Pro

**Miscellaneous**
- Scroll in copy mode: `Ctrl+b, [` (Navigate using arrow keys, PgUp, PgDn; to exit copy mode, press `q`)
- Reload tmux configuration: `tmux source-file ~/.tmux.conf`

Please note that these commands are based on the default `tmux` bindings and your personal configuration might override some of them.