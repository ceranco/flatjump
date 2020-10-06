# flatjump

This is a very simple script that will try to mimic the excellent [jumpapp](https://github.com/mkropat/jumpapp) for flatpak applications.

The usage is simply:
```bash
flatjump <NAME>
```

The script will search for an open flatpak application with the given name. If it finds it it will focus it, if not it will open a new instance.

## Setup

Simply clone the repo and run the script:
```bash
git clone https://github.com/ceranco/flatjump.git
cd flatjump
./flatjump <NAME>
```

If you want to use the script from a shortcut, the easiest way is to symlink the script to **/usr/bin/**:
```bash
ln -s /home/ceranco/projects/flatjump/flatjump /usr/bin/flatjump
```
and then simply use it in the shortcut: `flatjump <NAME>`
