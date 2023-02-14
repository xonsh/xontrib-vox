# xontrib-vox
Python virtual environment manager for xonsh.

```xsh
xontrib load vox
```
```
usage: vox [-h] {new,create,activate,workon,enter,deactivate,exit,list,ls,remove,rm,delete,del,info,runin,runin-all,toggle-ssp,wipe,project-set,project-get,upgrade} ...

Vox is a virtual environment manager for xonsh.

options:
  -h, --help
                        show this help message and exit

commands:
  {new,create,activate,workon,enter,deactivate,exit,list,ls,remove,rm,delete,del,info,runin,runin-all,toggle-ssp,wipe,project-set,project-get,upgrade}
    new (create)
                        Create a virtual environment in $VIRTUALENV_HOME with python3's ``venv``.
    activate (workon, enter)
                        Activate a virtual environment.
    deactivate (exit)
                        Deactivate the active virtual environment.
    list (ls)
                        List available virtual environments.
    remove (rm, delete, del)
                        Remove virtual environments.
    info
                        Prints the path for the supplied env
    runin
                        Run the command in the given environment
    runin-all
                        Run the command in all environments found under $VIRTUALENV_HOME
    toggle-ssp
                        Controls whether the active virtualenv will access the packages
                        in the global Python site-packages directory.
    wipe
                        Remove all installed packages from the current (or supplied) env.
    project-set
                        Bind an existing virtualenv to an existing project.
    project-get
                        Return a virtualenv's project directory.
    upgrade
                        Upgrade the environment directory to use this version
                        of Python, assuming Python has been upgraded in-place.

                        WARNING: If a virtual environment was created with symlinks or without PIP, you must
                        specify these options again on upgrade.
```
