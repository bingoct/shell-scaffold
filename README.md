## Introduction
shell-scaffold is a CLI simple shell scaffold.

### FIlE Tree
```plaintext
shell-scaffold
├── bin                 # a shell app templates
├── scripts             # sub command
├── shell_completion    # tab completion tempaltes
└── utils
    ├── alias
    └── functions
```


### Before write code
You should change the `bin/shell-scaffold` line 20 `APP_ROOT` to another name, like `foo`.
```bash
➜ sed -i "s/APP_ROOT/foo/" bin/shell-scaffold
```
And add `foo` to your environment.
```bash
➜ echo "export foo=$(pwd)" >>$HOME/.bashrc
```

### Prepare sub command
```plaintext
➜ ./bin/shell-scaffold
Description:
  shell-scaffold is a CLI simple shell scaffold
Usage:
  shell-scaffold [command]
Commands:
  version      - print version
  renew        - tool self-renewal
  implode      - uninstall this tool
  completion   - auto tab completion
  -h, help     - show usage text
```
