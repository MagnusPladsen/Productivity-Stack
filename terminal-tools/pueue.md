# pueue

> Queue and manage long-running shell commands with a persistent background daemon.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/Nukesor/pueue)

## Install

### macOS
```bash
brew install pueue
```

### Linux
```bash
# Cargo
cargo install --locked pueue

# Arch Linux
sudo pacman -S pueue
```

### Windows
```bash
# Scoop
scoop install pueue

# Cargo
cargo install --locked pueue
```

## Overview

pueue runs a daemon (`pueued`) in the background that manages a queue of shell commands. You can add tasks, control concurrency, pause/resume, retry on failure, and inspect logs — all without keeping a terminal open. The queue and logs survive crashes and system restarts.

```bash
# Start the daemon (once)
pueued -d

# Add a task to the queue
pueue add "sleep 10 && echo done"

# Add a task and label it
pueue add --label build "cargo build --release"

# Check queue status
pueue status

# Follow logs of a running task
pueue follow 0

# Run multiple tasks in parallel
pueue parallel 3

# Pause and resume the queue
pueue pause
pueue start

# Retry a failed task
pueue restart 2
```

Tasks are executed in their original working directory with the environment variables captured at add-time.
