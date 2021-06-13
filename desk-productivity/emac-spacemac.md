# ‎Emac

 Convenient key bindings are located under the prefix `SPC f e` to quickly navigate between `Emacs` and Spacemacs specific files.

| Key Binding | Description |
| :--- | :--- |
| `SPC f e c` | open `ido` in the `contrib` folder |
| `SPC f e d` | open the spacemacs dotfile \(`~/.spacemacs`\) |
| `SPC f e D` | open `ediff` buffer of `~/.spacemacs` and `.spacemacs.template` |
| `SPC f e f` | discover the `FAQ` using `helm` |
| `SPC f e i` | open the all mighty `init.el` |
| `SPC f e R` | resync the dotfile with spacemacs |
| `SPC f e v` | display and copy the spacemacs version |

 – \#\# Comment SPC ; comment operator SPC c y comment and yank SPC c p comment paragraphs

 – \#\# Find files SPC ff: find files or url SPC pf: find file in project SPC ph: search in a project with helm SPC bb: search in buffers

 – \#\# Search in files SPC ss /: search with evil

 – \#\# Window SPC w = balance split windows SPC w c close a window SPC w c close a window SPC w C delete another window using ace-delete-window SPC w d toggle window dedication \(dedicated window cannot be reused by a mode\) SPC w \[hjkl\] move to window SPC w \[HJKL\] move the window SPC w s or SPC w - horizontal split SPC w S horizontal split and focus new window SPC w u undo window layout \(used to effectively undo a closed window\) SPC w U redo window layout SPC w v or SPC w / vertical split SPC w V vertical split and focus new window SPC w w cycle and focus between windows SPC w m maximize/minimize a window \(maximize is equivalent to delete other windows\) SPC w M maximize/minimize a window, when maximized the buffer is centered

 – \#\# buffer SPC TAB switch to alternate buffer in the current window \(switch back and forth\) SPC b b switch to a buffer using helm SPC b d kill the current buffer \(does not delete the visited file\) SPC b e erase the content of the buffer \(ask for confirmation\) SPC b h open **spacemacs** home buffer SPC b k kill a buffer SPC b K kill all buffers except the current one

 – \#\# Project `projectile` commands start with p:

| Key Binding | Description |
| :--- | :--- |
| `SPC p !` | run shell command in root |
| `SPC p &` | run async shell command in root |
| `SPC p a` | toggle between implementation and test |
| `SPC p b` | switch to project buffer |
| `SPC p c` | compile project using `projectile` |
| `SPC p d` | find directory |
| `SPC p D` | open project root in `dired` |
| `SPC p f` | find file |
| `SPC p G` | regenerate the project's `etags` / `gtags` |
| `SPC p h` | find file using `helm` |
| `SPC p I` | invalidate the projectile cache |
| `SPC p k` | kill all project buffers |
| `SPC p o` | run `multi-occur` |
| `SPC p p` | switch project |
| `SPC p r` | open a recent file |
| `SPC p R` | replace a string |
| `SPC p s` | see Searching in a project |
| `SPC p t` | open `NeoTree` in `projectile` root |
| `SPC p T` | find test files |
| `SPC p v` | open project root in `vc-dir` or `magit` |
| `SPC p y` | find tags |
| `SPC /` | search in project with the best search tool available |
| `SPC s a p` | run `ag` |
| `SPC s g p` | run `grep` |
| `SPC s k p` | run `ack` |
| `SPC s t p` | run `pt` |

 – \#\# errors SPC e n go to the next error SPC e p go to the previous error

 – \#\# Quit SPC q q Quit Emacs and kill the server, prompt for changed buffers to save SPC q Q Quit Emacs and kill the server, lose all unsaved changes. SPC q r Restart both Emacs and the server, prompting to save any changed buffers SPC q s Save the buffers, quit Emacs and kill the server SPC q z Kill the current frame – \#\# Ruby on rails

| Key binding | Description |
| :--- | :--- |
| `SPC m r f a` | find localization file |
| `SPC m r f c` | find controller |
| `SPC m r f e` | find environment file |
| `SPC m r f f` | find feature |
| `SPC m r f h` | find helper |
| `SPC m r f i` | find initializer |
| `SPC m r f j` | find javascript file |
| `SPC m r f l` | find library |
| `SPC m r f m` | find model |
| `SPC m r f n` | find migration |
| `SPC m r f o` | find log |
| `SPC m r f p` | find spec file |
| `SPC m r f r` | find rake task |
| `SPC m r f s` | find stylesheet file |
| `SPC m r f t` | find test |
| `SPC m r f u` | find fixture |
| `SPC m r f v` | find view |
| `SPC m r f y` | find layout |
| `SPC m r f @` | find mailer |
| `SPC m r g c` | go to current controller |
| `SPC m r g d` | go to DB schema |
| `SPC m r g e` | go to DB seeds |
| `SPC m r g h` | go to current helper |
| `SPC m r g j` | go to current javascript |
| `SPC m r g g` | go to Gemfile |
| `SPC m r g m` | go to current model |
| `SPC m r g n` | go to current migration |
| `SPC m r g p` | go to current spec |
| `SPC m r g r` | go to routes |
| `SPC m r g s` | go to current stylesheet |
| `SPC m r g t` | go to current test |
| `SPC m r g u` | go to current fixture |
| `SPC m r g v` | go to current view |
| `SPC m r g z` | go to spec helper |
| `SPC m r g .` | go to file at point \(faster but less powerful than `SPC m g g`\) |

