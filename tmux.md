# Shortcuts
## Sessions
Start a New Session:  
- `tmux`
- `tmux new`
- `tmux new-session`
- `:new`

Start a new session or attach to an existing session named mysession:  
- `tmux new-session -A -s mysession`

Start a new session with the name mysession  
- `tmux new -s mysession`
- `:new -s mysession`

Kill/delete the current session:  
- `:kill-session`

Kill/delete session mysession  
- `tmux kill-ses -t mysesssion`
- `tmux kill-session -t mysession`

Kill/delete all sessions but the current  
- `tmux kill-session -a`

Kill/delete all sessions but mysession  
- `tmux kill-session -a -t mysession`

Rename current session  
- `ctrl+b, $`

Detach from session  
- `ctrl+b, d`

Detach others on the session  
- `:attach -d`

List all sessions  
- `tmux ls`
- `tmux list-sessions`
- `ctrl+b, s`

Attach to last session  
- `tmux a`
- `tmxu at`
- `tmux attach`
- `tmux attach-session`

Session and Window Preview  
- `ctrl+b, w`

Move to previous session  
- `ctrl+b, (`

Move to the next session  
- `ctrl+b, )`

Attach to a session with the name mysession  
- `tmux a -t mysession`
- `tmux at -t mysession`
- `tmux attach -t mysession`
- `tmux attach-session -t mysession`

Session and Window Preview  
- `ctrl+b, w`

Move to previous session  
- `ctrl+b, (`

Move to the next session  
- `ctrl+b, )`

## Windows
## Panes
## Copy Mode
## Misc.
## Help
