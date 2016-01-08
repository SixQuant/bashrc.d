# .bash_inc

## Setup
Just download .bash_inc to ~/
and append below code to ~/.bash_profile

```bash
# Load extra bash config
for file in ~/.bash_inc/{path,bash_prompt,exports,aliases,functions,extra}; do
    [ -r "$file" ] && [ -f "$file" ] && source "$file";
done;
unset file;
```
