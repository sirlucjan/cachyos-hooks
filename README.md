# cachyos-hooks

Pacman hooks for setting up system identification files and other features of Cachy OS.

File name | Description
:--- | :---
cachyos-hooks-runner | Fixes files like `os-release`, `lsb-release`, `issues` for Cachy OS.
cachyos-hooks.hook | Runs `cachyos-hooks-runner` after the `cachyos-hooks` package is updated.
lsb-release.hook | Runs `cachyos-hooks-runner` after package `lsb-release` has been updated.
os-release.hook | Runs `cachyos-hooks-runner` after package `filesystem` has been updated.
cachyos-reboot-required | Notifies user to reboot after essential system files have been updated.
cachyos-check-reboot-required | Filters a selection of kernel targets to `cachyos-reboot-required`.
cachyos-reboot-required.hook | Runs `cachyos-reboot-required` after any listed essential system files have been updated.
cachyos-reboot-required.hook | Runs `bootctl --no-variables --graceful update` after systemd has been updated.
