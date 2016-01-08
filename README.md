# .bash_inc


append below code to ~/.bash_profile

# Load extra bash config
for file in ~/.bash_inc/{path,bash_prompt,exports,aliases,functions,extra}; do
    [ -r "$file" ] && [ -f "$file" ] && source "$file";
done;
unset file;
