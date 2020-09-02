# polybar-git-checker

A polybar script to check git repositories from a root directory.

![example](screenshots/example.png)

Add to your polybar config:

```sh
...

[module/repository-checker]
type = custom/script
exec = ~/.config/polybar/git-status-checker.sh
exec-if = true
tail = true
interval = 60
format = <label>
label = %output%
format-underline = #282a36
click-left = %label%

...
```

