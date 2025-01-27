# ZetaSQLite CLI

`zetasqlite-cli` is a CLI tool for directly executing ZetaSQL queries by specifying a database, allowing you to execute queries interactively like the sqlite3 CLI. It also supports query input from standard input.

## Install

```console
$ go install github.com/goccy/go-zetasqlite/cmd/zetasqlite-cli@latest
```

## How to use

```console
Usage:
  zetasqlite-cli [OPTIONS]

Application Options:
      --raw        specify the raw query mode. write sqlite3 query directly. this is a debug mode for developers
      --history=   specify the history file for used queries (default: .zetasqlite_history)
      --autoindex  specify the auto index mode. automatically create an index when creating a table
      --explain    specify the explain mode. show results using sqlite3's explain query plan instead of executing the query

Help Options:
  -h, --help     Show this help message
```

## Commands

- `.quit` : quit CLI
- `.exit` : quit CLI
- `.tables` : show all tables
- `.functions` : show all functions
- `.autoindex` : automatically create an index when creating a table
- `.explain` : show results using sqlite3's explain query plan instead of executing the query
