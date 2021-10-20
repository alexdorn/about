## Editing ##
```{command} {text object or motion}```
```
{d(delete/cut} | c(change) | y(yank/copy) | p (paste) | v (visually select} {i(inside) | a(all) | t(til)}
```
### Examples ###
- **diw** {delete in word} - delete entire word, current position doesn't matter. **dw** deletes only after cursor!
- **caw** - change all word
- **di(** {delete inside <symbol> - delete content inside parentheses/bracets/etc
- **dt\<symbol\>** - delete until \<symbol\>, not including the \<symbol\> itself
- **df\<symbol\>** - delete until \<symbol\>, including
- **va"** - visually select all inside doublequotes

## Repetition ##
  
- **.** (single dot) - repeats the latest command
  
## Anchors ##

- **D / C** - delete/change until end of line, same as **d$/c$**
- **^ / $** - move to the beginning/end of line
- **I / A** - move to the beginnin/end of line and insert
- **O / o** - insert new line before/after
- **P / p** - paste before/after

## Navigation ##
- **H** – Go to the first line of current screen.
- **M** – Go to the middle line of current screen.
- **L** – Go to the last line of current screen.
- **ctrl+f** – Jump forward one full screen.
- **ctrl+b** – Jump backwards one full screen
- **ctrl+d** – Jump forward (down) a half screen
- **ctrl+u** – Jump back (up) one half screen

## Search ##
- **f | F\<symbol>** – Forward/reverse search in string under cursor and jump TO \<symbol>
- **t | T\<symbol>** – Forward/reverse search in string under cursor and jump BEFORE \<symbol>
- **/ | ?\<pattern>** - Forward/reverse search throught all file. Use **n|N** for jumping between search results
  
  
## Macros ##
Macro - sequence of commands you want to repeat

**Record macro**
```
  q{reqister}
  (do the things)
  q
```
**Play macro**
```
  @{register}
```  
