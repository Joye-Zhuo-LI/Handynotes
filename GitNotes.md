# Add Files greater than 100MB to gitignore
```git
find . -size +100M | cat >> .gitignore
```
