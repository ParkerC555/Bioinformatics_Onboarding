# Self‑guided Command Line Tutorial
Estimated time: ~20 minutes. Assumes you're using a Unix-like shell (bash/zsh) in the VS Code terminal.

1) Basics & orientation
- `pwd`                # show current directory
- `ls -lah`            # list files (flags: -l long, -a all, -h human-readable)
- `cd DIR`             # change directory; `cd ..` (up), `cd ~` (home), `cd -` (previous)

2) Tab completion & history
- Press `Tab` to autocomplete file/dir names.
- Use `Up/Down` arrows or `Ctrl+R` to search command history.

3) Create files and folders
- `mkdir my_project`
- `cd my_project`
- `touch notes.txt script.sh`
- `ls`

4) View and edit files
- `cat notes.txt`
- `less notes.txt`
- `open notes.txt`     # on Mac, or open file in VS Code via the editor
- Use VS Code to edit files (preferred for this course).

5) Copy, move, remove
- `cp notes.txt notes.bak`
- `mv notes.bak archive/`
- `rm file_to_remove`   # be careful; use `rm -i` for interactive delete
- `rm -r directory/`    # recursive remove (dangerous)

6) Make and run a simple script
- Create `script.sh`:
  ```bash
  #!/bin/bash
  echo "Hello from script"
  ```
- `chmod +x script.sh`
- `./script.sh`

7) Flags, help & man pages
- `command --help`      # quick usage
- `man ls`              # detailed manual (if available)

8) Pipes and redirects
- `ls | grep ".md"`     # filter ls output
- `echo -e "one\ntwo" > sample.txt`
- `cat sample.txt | grep one`

9) Searching
- `grep -n "pattern" *.txt`
- `find . -name '*.md'`

10) Useful shortcuts
- `Ctrl+C`  stop current command
- `Ctrl+D`  close shell / log out
- `Ctrl+L`  clear screen

11) Quick git primer (in a repo)
- `git status`
- `git add file`
- `git commit -m "short message"`
- `git push`

Practice exercises:
- Create a folder `practice`, inside it create `demo.sh` that prints the working dir and lists files. Make it executable and run it.
- Create two files, search for a word across them with grep, and save the results to `results.txt`.

If you want this tailored to your OS (Windows Git Bash vs Mac/Linux), level (beginner/intermediate), or duration (10/20/30 mins), tell me which and I'll adapt it.

