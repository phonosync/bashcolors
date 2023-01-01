# bashcolors
Prompt and ls-colors customisation for bash in the wsl terminal
## ls-colors
```bash
dircolors --print-database > ~/.dircolors
```
Then edit `~/.dircolors`

list of all the keys:
http://www.bigsoft.co.uk/blog/2008/04/11/configuring-ls_colors

```bash
source .bashrc
```
`.dircolors` is loaded in the line: 
```bash
test -r ~/.dircolors && eval "$(dircolors -b ~/.dircolors)" || eval "$(dircolors -b)"
```
## prompt
In the `.bashrc`-file
with color:
`PS1='\[\033[34m\]\w\[\033[00m\]\$ '`
without:
`PS1='\w\$ '`
