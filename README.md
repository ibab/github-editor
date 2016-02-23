# github-editor

Edit files in your github repo with $EDITOR.

Install dependencies with
```bash
pip install --user -r requirements.txt
```

Run
```bash
./ged yourname/yourrepo todo.md
```
This opens up a file in your `$EDITOR`.
If you modify and save the file, the change will get automatically committed to
your github repository.

If you don't change anything in the file, or if you leave it empty, nothing will be committed.
The script also adds yaml frontmatter to the beginning of the file:
```
---
message: Update todo.md
---
```
This allows you to set the commit message.

I use this to quickly edit my notes and todo lists in a special repo.
