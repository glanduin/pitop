# pitop

Interactive terminal monitor for Raspberry Pi 5.

Shows CPU/GPU/PMIC temperatures, clock speed, network throughput, filesystem
usage, per-core CPU bars, and processes grouped by CPU or memory. Filesystem
rows prefer the filesystem label and fall back to the device name; unmounted
filesystems are omitted.

## Usage

```sh
pitop
```

An interactive PTY is required; over SSH use `ssh -t`. Set `NO_COLOR=1` for
monochrome output. ANSI escape sequences are used automatically when terminfo
is unavailable. Press `c` / `m` to change process grouping, and `Esc` to quit.

## Install

```sh
sudo install -m 755 -o root -g root pitop /usr/local/bin/pitop
```
