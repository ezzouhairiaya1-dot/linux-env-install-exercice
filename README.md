# linux-env-install-exercice

# Linux environment setup (shell and bash scripting exercise)

A bash script that sets up a small Python development environment on Linux or macOS.

## Files
- `env_install.sh`: the automation script

## What the script does
1. `pretty_print`: prints a message between blank lines with printf
2. Detects the operating system with the OSTYPE variable (linux or macos)
3. Checks that python3 is installed, installs it with apt or brew if not
4. Checks that pip is available and shows its version
5. Installs Jupyter Notebook (apt on Linux, brew on macOS)
6. On macOS only, runs brew doctor to check Homebrew

## How to run
    chmod +x env_install.sh
    ./env_install.sh

Tested on Ubuntu with WSL. Result: Python 3.14.4, pip 25.1.1, Jupyter Notebook 6.4.13.

## Shell setup (part 1)
- Shell: bash (/bin/bash), checked with `echo $SHELL`
- Framework: Oh My Bash, with the git plugin enabled in ~/.bashrc
- Alias test: `gst` runs `git status`

## What does the source command do?
`source file` runs the commands of a file in the current shell. After editing ~/.bashrc, `source ~/.bashrc` applies the changes without restarting the terminal.

## Note
This script was written with AI assistance. I tested it and reviewed it myself.
