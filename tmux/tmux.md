[toc]

# TMUX Commands
## Sessions
| Description | TMUX Command | Shortcut |
|-------------|--------------|---------|
| Start a New Session | `tmux`, `tmux new`, `tmux new-session`, `:new` | - |
| Start a new session or attach to existing session named mysession | `tmux new-session -A -s mysession` | - |
| Start a new session with the name mysession | `tmux new -s mysession`, `:new -s mysession` | - |
| Kill/delete the current session | `:kill-session` | - |
| Kill/delete session mysession | `tmux kill-ses -t mysession`, `tmux kill-session -t mysession` | - |
| Kill/delete all sessions but the current | `tmux kill-session -a` | - |
| Kill/delete all sessions but mysession | `tmux kill-session -a -t mysession` | - |
| Rename current session | - | `ctrl+b, $` |
| Detach from session | - | `ctrl+b, d` |
| Detach others on the session | `:attach -d` | - |
| List all sessions | `tmux ls`, `tmux list-sessions` | `ctrl+b, s` |
| Attach to last session | `tmux a`, `tmux at`, `tmux attach`, `tmux attach-session` | - |
| Session and Window Preview | - | `ctrl+b, w` |
| Move to previous session | - | `ctrl+b, (` |
| Move to next session | - | `ctrl+b, )` |
| Attach to a session with the name mysession | `tmux a -t mysession`, `tmux at -t mysession`, `tmux attach -t mysession`, `tmux attach-session -t mysession` | - |

## Windows
| Description | TMUX Command | Shortcut |
|-------------|--------------|---------|
| Start a new session with the name mysession and window mywindow | `tmux dnew -s mysession -n mywindow` | - |
| Create a New window | - | `ctrl+b, c` |
| Rename current window | - | `ctrl+b, ,` |
| Close current window | - | `ctrl+b, &` |
| List windows | - | `ctrl+b, w` |
| Prev window | - | `ctrl+b, p` |
| Next window | - | `ctrl+b, n` |
| Switch to window by number | - | `ctrl+b, 0...9` |
| Toggle to last active window | - | `ctrl+b, l` |
| Reorder window, swap window number 2(src) and 1(dst) | `swap-window -s 2 -t 1` | - |
| Move current window to the left by one position | `swap-window -t -1` | - |
| Move window from source to target | `move-window -s src_ses:win -t target_ses:win`, `movew -s foo:0 -t bar:9`, `movew -s 0:0 -t 1:9` | - |
| Reposition window in the current session | `move-window -s src_session:src_window`, `movew -s 0:9` | - |
| Renumber windows to remove gap in the sequence | `move-window -r`, `movew -r` | - |

## Panes
| Description | TMUX Command | Shortcut |
|-------------|--------------|---------|
| Toggle last active pane | - | `ctrl+b, ;` |
| Split the current pane vertically (horizontal layout) | `split-window -h` | `ctrl+b, "` |
| Split the current pane horizontally (vertical layout) | `split-window -v` | `ctrl+b, %` |
| Join two windows as panes | `join-pane -s 2 -t 1` | - |
| Move pane from one window to another | `join-pane -s 2.1 -t 1.0` | - |
| Move the current pane left | - | `ctrl+b, {` |
| Move the current pane right | - | `ctrl+b, }` |
| Switch to pane in direction | - | `ctrl+b, arrow keys` |
| Toggle synchronize-panes (send command to all panes) | `setw synchronize-panes` | `ctrl+b, :setw synchronize-panes` |
| Toggle between pane layouts | - | `ctrl+b, space` |
| Switch to next pane | - | `ctrl+b, o` |
| Show pane numbers | - | `ctrl+b, q` |
| Switch/select pane by number | - | `ctrl+b, q (then number)` |
| Toggle pane zoom | - | `ctrl+b, z` |
| Convert pane into a window | - | `ctrl+b, !` |
| Resize current pane height | - | `ctrl+b, ctrl+↑`, `ctrl+b, ctrl+↓` |
| Resize current pane width | - | `ctrl+b, ctrl+←`, `ctrl+b, ctrl+→` |
| Close current pane | - | `ctrl+b, x` |

## Copy Mode
| Description | TMUX Command | Shortcut |
|-------------|--------------|---------|
| Use vi keys in buffer | `setw -g mode-keys vi` | - |
| Enter copy mode | - | `ctrl+b, [` |
| Enter copy mode and scroll one page up | - | `ctrl+b, PgUp` |
| Quit mode | - | `q` |
| Go to top line | - | `g` |
| Go to bottom line | - | `G` |
| Scroll up | - | `ctrl+u` |
| Scroll down | - | `ctrl+d` |
| Move cursor left | - | `h` |
| Move cursor down | - | `j` |
| Move cursor up | - | `k` |
| Move cursor right | - | `l` |
| Move cursor forward one word at a time | - | `w` |
| Move cursor backward one word at a time | - | `b` |
| Search forward | - | `/` |
| Search backward | - | `?` |
| Next keyword occurrence | - | `n` |
| Previous keyword occurrence | - | `N` |
| Start selection | - | `space` |
| Clear selection | - | `esc` |
| Copy selection | - | `enter` |
| Paste contents of buffer_0 | - | `ctrl+b, ]` |
| Display buffer_0 contents | `show-buffer` | - |
| Copy entire visible contents of pane to a buffer | `capture-pane` | - |
| Show all buffers | `list-buffers` | - |
| Show all buffers and paste selected | `choose-buffer` | - |
| Save buffer contents to buf.txt | `save-buffer buf.txt` | - |
| Delete buffer_1 | `delete-buffer -b 1` | - |

## Misc
| Description | TMUX Command | Shortcut |
|-------------|--------------|---------|
| Enter command mode | - | `ctrl+b, :` |
| Set OPTION for all sessions | `set -g OPTION` | - |
| Set OPTION for all windows | `setw -g OPTION` | - |
| Enable mouse mode | `set -g mouse on` | - |

## Help
| Description | TMUX Command | Shortcut |
|-------------|--------------|---------|
| List key bindings (shortcuts) | `tmux list-keys`, `list-keys` | - |
| Show every session, window, pane, etc. | `tmux info` | - |


