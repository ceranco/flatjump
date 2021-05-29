# flatjump

This is a very simple script that tries to mimic the excellent [jumpapp](https://github.com/mkropat/jumpapp) for flatpak applications.

The usage is simply:
```bash
flatjump <NAME> [<SEARCH-EXPR>]
```

For example:
```bash
flatjump slack
```

The script will search for an open flatpak application with the given name (case-insensitive). 
* If found, it will be focused. 
* If not, a new instance will be opened.

To prevent confusion between open applications that contain <NAME> in the title, you can give an optional <SEARCH-EXPR> (case-insensitive) to be used
when searching through all open windows.

## Setup

Simply clone the repo and run the script:
```bash
git clone https://github.com/ceranco/flatjump.git
cd flatjump
./flatjump <NAME>
```

If you want to use the script in a shortcut, the easiest way is to symlink the script to **/usr/bin/**:
```bash
ln -s /home/ceranco/projects/flatjump/flatjump /usr/bin/flatjump
```
and then simply use it in the shortcut: `flatjump <NAME>`
