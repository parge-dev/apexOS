# ApexOS

**A small experimental text-based operating system built with C++.**

<escape>⚠️</escape> **BETA SOFTWARE — NOT A RELEASE**

ApexOS is an experimental operating system project designed to explore low-level programming, operating system development, and command-line interfaces.

---

## Current Version

| Information | Details |
|---|---|
| OS Name | ApexOS |
| Version | 1.0 |
| Build | Beta |
| Test | 1 |
| Language | C++ |
| Architecture | x86_64 |
| Bootloader | Limine |
| Status | Experimental |

## Features

- Text-based user interface
- Keyboard support
- Command-line shell
- Custom username
- Built-in commands
- Beta developer commands
- Reboot command
- Custom ApexOS startup screen
- System information commands

## Commands

| Command | Description |
|---|---|
| `help` | Show available commands |
| `clear` | Clear the screen |
| `cls` | Clear the screen |
| `about` | About ApexOS |
| `version` | Show OS version |
| `ver` | Show OS version |
| `name` | Change username |
| `whoami` | Show current username |
| `echo` | Display text |
| `banner` | Show ApexOS banner |
| `ls` | Show virtual files |
| `pwd` | Show current directory |
| `uname` | Show system information |
| `motd` | Show message of the day |
| `credits` | Show project credits |
| `reboot` | Restart ApexOS |
| `shutdown` | Shutdown command |

### Developer Commands

ApexOS Beta includes a `dev` command with experimental developer tools.

Try:

```bash
dev help
```

Developer commands are currently intended for beta testing.

---

## Tested Hardware & Environment

ApexOS has been built and tested in the following environment.

### Host Device Specifications

| Specification | Details |
|---|---|
| Operating System | Debian GNU/Linux 13 (Trixie) |
| Kernel | 6.6.147-09792-gc3031f3e2ec6 |
| Architecture | x86_64 |
| Device Model | crosvm |
| Manufacturer | ChromiumOS |
| CPU | Intel Celeron N4020 @ 1.10GHz |
| Total RAM | 2.7 GiB |
| Available RAM at test | 1.1 GiB |
| Swap | 0 B |

### Virtual Machine Specifications

| Specification | Details |
|---|---|
| Virtualization Software | QEMU |
| Architecture | x86_64 |
| Allocated RAM | 512 MB |
| Boot Media | ApexOS ISO |
| Bootloader | Limine |
| Virtual Machine Type | x86_64 |

### Testing Notes

- Built inside Debian GNU/Linux 13.
- Tested on a ChromeOS Linux environment (Crostini).
- Host processor: Intel Celeron N4020.
- Tested using QEMU with 512 MB of virtual RAM.
- Booted using the Limine bootloader.

These are tested configurations, not minimum system requirements.

---

## Building ApexOS

ApexOS uses the Limine C++ template.

### Requirements

- C++ compiler
- Make
- xorriso
- QEMU (optional, for testing)

### Build

Clone the repository:

```bash
git clone https://github.com/parge-dev/ApexOS.git
cd ApexOS
```

Build the operating system:

```bash
make clean && make
```

### Run in QEMU

```bash
qemu-system-x86_64 -cdrom template-x86_64.iso -m 512M -boot d
```

---

## Project Status

ApexOS is currently in early beta development.

Features may be incomplete, change, or contain bugs.

**This is not a stable release.**

More features and improvements are planned for future versions.

---

## Credits

- **Developer:** parge-dev
- **Bootloader:** Limine
- **Project:** ApexOS
- **Language:** C++

Made by **parge-dev on GitHub**.

---

**Thanks for checking out ApexOS!**
