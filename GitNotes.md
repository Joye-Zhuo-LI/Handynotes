# Add Files greater than 100MB to gitignore
```git
find . -size +100M | cat >> .gitignore
find . -size +100M | sed 's|^\./||g' | cat >> .gitignore
find . -size +100M | sed 's|^\./||g' | cat >> .gitignore; awk '!NF || !seen[$0]++' .gitignore
sort -u .gitignore -o .gitignore
```
