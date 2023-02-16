<p align="center">
Python virtual environment manager for xonsh shell.
</p>

<p align="center">  
If you like the idea click ⭐ on the repo and <a href="https://twitter.com/intent/tweet?text=Nice%20xontrib%20for%20the%20xonsh%20shell!&url=https://github.com/xonsh/xontrib-vox" target="_blank">tweet</a>.
</p>


## Installation

To install use pip:

```bash
xpip install xontrib-vox
# or: xpip install -U git+https://github.com/xonsh/xontrib-vox
```

## Usage

This package contains three xontribs:
* `vox` - Python virtual environment manager for xonsh.
* `autovox` - Manages automatic activation of virtual environments.
* `voxapi` - API for Vox, the Python virtual environment manager for xonsh.

### vox

Python virtual environment manager for xonsh.

```bash
xontrib load vox
vox --help
```

### autovox

Manages automatic activation of virtual environments.

```bash
xontrib load autovox
```

This coordinates multiple automatic vox policies and deals with some of the
mechanics of venv searching and chdir handling.

This provides no interface for end users.

Developers should look at XSH.builtins.events.autovox_policy

### voxapi

API for Vox, the Python virtual environment manager for xonsh.

```bash
xontrib load voxapi
```

Vox defines several events related to the life cycle of virtual environments:

* `vox_on_create(env: str) -> None`
* `vox_on_activate(env: str, path: pathlib.Path) -> None`
* `vox_on_deactivate(env: str, path: pathlib.Path) -> None`
* `vox_on_delete(env: str) -> None`


## Credits

This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
