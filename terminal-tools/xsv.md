# xsv

> A fast CSV command-line toolkit for slicing, filtering, joining, and analyzing CSV files.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/BurntSushi/xsv)

## Install

### macOS
```bash
brew install xsv
```

### Linux
```bash
cargo install xsv
```

### Windows
```bash
cargo install xsv
```

## Overview

xsv is a suite of CSV commands that are fast enough to work on large files. It can slice, filter, aggregate, join, flatten, and index CSV data from the command line without loading everything into memory.

> **Note:** The repository was archived by the author in April 2025 and is now read-only. The tool remains functional and available, but is no longer actively maintained. Consider [qsv](https://github.com/jqnatividad/qsv) as an actively maintained fork.

```bash
# Show headers
xsv headers data.csv

# Count rows
xsv count data.csv

# Select specific columns
xsv select name,age data.csv

# Filter rows
xsv search -s status "active" data.csv

# Sort by column
xsv sort -s name data.csv

# Compute statistics
xsv stats data.csv

# Join two CSV files
xsv join id users.csv user_id orders.csv
```

## Alternatives
- [jq](jq.md)
