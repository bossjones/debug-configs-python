# debug-configs-python
Debug configs (eg .pdbrc, pythonrc, .pythonstart, .inputrc, .fancycompleterrc.py, etc ) used by bossjones projects / repositories.

# bossjones debugConfigs

This repository contains debug configs for different python modules. eg:

```bash
total 40
drwxr-xr-x 10 ultron staff  320 May 30 12:14 .
drwxr-xr-x  6 ultron staff  192 May 30 12:12 ..
-rw-r--r--  1 ultron staff 1236 May 30 12:08 .pyenv_compile_env_brew
-rw-r--r--  1 ultron staff 5316 Oct  1  2018 .ptpython_config.py
-rw-r--r--  1 ultron staff 4462 Oct  1  2018 .pdbrc.py
-rw-r--r--  1 ultron staff  151 Oct  1  2018 .fancycompleterrc.py
-rw-r--r--  1 ultron staff 2487 Sep 24  2018 .pythonstart
-rw-r--r--  1 ultron staff 2934 Sep 24  2018 .pdbrc
-rw-r--r--  1 ultron staff  279 Sep 24  2018 .inputrc
-rw-r--r--  1 ultron staff  171 Sep 24  2018 .pythonrc
```

Configs are grouped in sub-directories by programming language.

## Usage

To use those configs, add this repository as a git subtree to the repository
where you want to utilize those configs. After that is done, update make
targets (or similar) to correctly pass path to the configs to the tools
in question.

```bash
git subtree add --prefix debug-configs-python https://github.com/bossjones/debug-configs-python.git master --squash
```

And once you want to pull changes / updates from the debug-configs-python repository:

```bash
git subtree pull --prefix debug-configs-python https://github.com/bossjones/debug-configs-python.git master --squash
```

# Inspiration

https://github.com/StackStorm/lint-configs
